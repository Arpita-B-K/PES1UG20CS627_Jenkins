#!/usr/bin/env groovy
pipeline{
  agent{
    docker{
      image 'jenkins:PES1UG20CS627'
    }
  }
  stages{
    stage('Clone repository'){
      steps{
        git branch: 'main',
        url: 'https://github.com/Arpita-B-K/PES1UG20CS627_Jenkins.git'
      }
    }
   
