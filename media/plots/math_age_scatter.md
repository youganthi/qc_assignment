p <- ggplot(bigclass, aes(x = age, y = Math)) +
  geom_point(color = '#0072B2', size = 3) +
  labs(title = 'Math Scores vs. Age', x = 'Age', y = 'Math Score') +
  theme_minimal() +
  theme(axis.title = element_text(size = 18),
        axis.text = element_text(size = 14),
        panel.background = element_rect(fill = 'white', color = NA))

p_plotly <- ggplotly(p)
