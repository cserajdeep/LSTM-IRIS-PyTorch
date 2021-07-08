# LSTM Model
```ruby
class LSTM(nn.Module):
  def __init__(self, num_classes, input_size, hidden_size, num_layers):
    super(LSTM, self).__init__()
    self.num_classes = num_classes
    self.num_layers = num_layers
    self.input_size = input_size
    self.hidden_size = hidden_size
    self.seq_length = seq_length
        
    self.lstm = nn.LSTM(input_size=input_size, hidden_size=hidden_size,
                            num_layers=num_layers, batch_first=True)
        
    self.fc = nn.Linear(hidden_size, num_classes)
```

# Area Under Curve
<img width="467" alt="lstmiris_auc" src="https://user-images.githubusercontent.com/18000553/124860445-4b54b900-dfcf-11eb-8cac-f686f96afb0f.png">

# LSTM IRIS PyTorch
