class AdsController < ApplicationController
  def index
    @ads = Ad.find(:all)
  end  
  
  def new
    @ad = Ad.new
  end
  
  def show
    @ad = Ad.find(params[:id])
  end
  
  def create
    @ad = Ad.new(params[:ad])
    @ad.save  
    redirect_to "/ads/#{@ad.id}"
  end
end
