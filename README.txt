#### Save model and run it later
## i think u can you 
torch.save(model.state_dict(), 'rl_model.pth') to save model and 
model = YourModel()  
model.load_state_dict(torch.load('rl_model.pth'))
to load it. Hope this helps.