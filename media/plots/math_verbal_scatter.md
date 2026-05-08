p <- ggplot(bigclass, aes(x = Math, y = Verbal)) +
  geom_point(color = '#0072B2', size = 3) +
  labs(title = 'Math Scores vs. Verbal Scores', x = 'Math Score', y = 'Verbal Score') +
  theme_minimal() +
  theme(axis.title = element_text(size = 18),
        axis.text = element_text(size = 14),
        panel.background = element_rect(fill = 'white', color = NA))

p_plotly <- ggplotly(p)
