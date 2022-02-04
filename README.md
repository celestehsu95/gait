# gait
We  used  a  Variational  Autoencoder  as  my  model. 
A  VAEhas three parts:
1.  An  encoder  that  that  learns  the  mean  and  variance  of  thelatent distribution.
2. A method of sampling from the distribution.
3. A decoder that can turn the sample back into an image.

Variational  Autoencoders  are  a  model  for  transforming  high-dimensional  data  into  a  lower-dimensional  space.  How  theywork  is  by  encoding  the  data  to  a  1-D  vector.  Then  decodethis vector to reconstruct the original data(IMU here). The lossbetween  the  generated data  and  the  original  data depends  onhow accurate the VAEs are. The more precise the VAEs are,the closer the generated data is to the original. VAE learn theprobability  distribution  parameters  from  the  data  came,  andhence  get  the  latent  variable.  The  encoder’s  job  is  to  receivethe data with multiple dimensions and generate a single vectorrepresenting the entire original data. This single vector is theso-called latent variables. Then the latent variables will be fedto the decoder. The decoder’s job is to reconstruct the originaldata, so it is just a reflection of the encoder.
