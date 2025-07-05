# ReviewGraph
ReviewGraph project with visualisation features. code and data to be shared here.


# {System Output Visualisation}
While the visualisation aspect was not the core focus of our study, we did find that the graph structure of our model has natural potential of being a useful data visualisation tool. 
 
Currently we developed several minor features for this graph visualisation, which lets the user sort the graph to show data they are specifically interested in. More features can easily be added in the future. 
 
Some of the current features are:
\begin{itemize}
    \item Show only reviews of a specific score or score range (2-4 for example).
    \item Show only the highest or lowest sentiment score reviews, hotels, or words
    \item When looking at only low sentiment reviews, the user can click on the review and see what the review is roughly about by looking at the connected nodes that show up on screen.
\end{itemize}

In Figure \ref{fig:system-visualisation} and Figure \ref{fig:system-visualisation-review} are some examples of how the visualisation currently works. Every node is interactable and when clicked on shows all the nodes it is connected to.

[fig:system-visualisation-review](https://github.com/aaronlifenghan/ReviewGraph/blob/main/review.png)

[fig:system-visualisation](https://github.com/aaronlifenghan/ReviewGraph/blob/main/visualization.png)



\begin{figure}[H]
    \centering
    \includegraphics[width=1\linewidth]{bachthesis2019/visualization.png}
    \caption{Example of a hotel and two negative sentiment reviews connected to it. The blue circle is the hotel, the green ones are the reviews, and the yellow ones are subjects/objects extracted from the review text. }
    \label{fig:system-visualisation}
\end{figure}

\begin{figure}[H]
    \centering
    \includegraphics[width=1\linewidth]{bachthesis2019/review.png}
    \caption{Example of review and all the nodes connected to it as well as the relationships between those nodes connected to it. The blue one is the hotel, the green one the review, and the yellow ones are subjects/object extracted from the review text. }
    \label{fig:system-visualisation-review}
\end{figure}

# Data Illustration

The distribution per rating score can be seen in Figure~\ref{fig:reviews_per_rating}.

[fig:reviews_per_rating](https://github.com/aaronlifenghan/ReviewGraph/blob/main/reviews_per_rating.png)

% \begin{figure}[t]
%     \centering
%     \includegraphics[width=0.5\textwidth]{bachthesis2019/reviews_per_rating.png}
%     \caption{Distribution of the number of reviews per rating score (1 to 5).}
%     \label{fig:reviews_per_rating}
% \end{figure}

The distribution of review lengths can be seen in Figure~\ref{fig:reviews_per_length}. 
Any reviews longer than 1000 words were removed from this chart for readability purposes.

[fig:reviews_per_length](https://github.com/aaronlifenghan/ReviewGraph/blob/main/review_length.png)
\begin{figure}[t]
    \centering
    \includegraphics[width=0.5\textwidth]{bachthesis2019/review_length.png}
    \caption{Distribution of reviews by their length}
    \label{fig:reviews_per_length}
\end{figure}

# {Appendix on key codes, more examples and evaluations}
[example of triples extracted, key codes, and overall 10fold cross-validation eval table](https://github.com/aaronlifenghan/ReviewGraph/blob/main/Appendix-triples-10folds.pdf)
