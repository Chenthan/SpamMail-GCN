# Spam Mails Detection Using GCN Algorithm
GCN is Convolutional Neural networks Based classification Algorithm. 
It uses a semi-supervised Learning approach. Also Some NLP techniques are also used

# Modules Used
-pickle

-pandas

-sklearn

-nltk

-numpy

-networkx

-collections

-tqdm

-pytorch

-matplotlib

# To run :
git clone https://github.com/Chenthan/SpamMail-GCN.git

Then create Folder named data and place your own Datasets

python classify.py [-h]

	[--train_data TRAIN_DATA (default: "./data/train.csv")] 
	[--infer_data INFER_DATA (default: "./data/infer.csv")]            
	[--max_vocab_len MAX_VOCAB_LEN (default: 7000)]  
	[--hidden_size_1 HIDDEN_SIZE_1 (default: 330)]
	[--hidden_size_2 HIDDEN_SIZE_2 (default: 130)]  
	[--batched BATCHED (default: 0)]  
	[--hidden HIDDEN (default: 8)]
	[--nb_heads NB_HEADS (default: 8)]
	[--tokens_length TOKENS_LENGTH (default: 200)] 
	[--num_classes NUM_CLASSES (default: 2)]
	[--train_test_split TRAIN_TEST_SPLIT (default: 0)]
	[--test_ratio TEST_RATIO (default: 0.1)] 
	[--batch_size BATCH_SIZE (default: 32)]      
	[--gradient_acc_steps GRADIENT_ACC_STEPS (default: 1)]
	[--max_norm MAX_NORM (default: 1)] 
	[--num_epochs NUM_EPOCHS (default: 1700)] 
	[--lr LR default=0.0031]
	[--use_cuda USE_CUDA] [--train TRAIN (default:1)]
	[--infer INFER (default: 0 (Infer input sentence labels from trained model))]
