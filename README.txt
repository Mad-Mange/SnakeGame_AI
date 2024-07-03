#### Save model and run it later
## i think u can you 
torch.save(model.state_dict(), 'rl_model.pth') to save model and 
model = YourModel()  
model.load_state_dict(torch.load('rl_model.pth'))
to load it. Hope this helps.



#### Export/Import Conda environments
## Export to file
conda env export --name pygame_env > environment.yml
## Import from file
conda env create -f environment.yml