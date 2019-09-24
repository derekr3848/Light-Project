# Light-Project
Xcode
//
//  ViewController.swift
//  Light V2
//
//  Created by Derek Rodriguez Martinez on 9/23/19.
//  Copyright © 2019 Derek Rodriguez Martinez. All rights reserved.
//

import UIKit

class ViewController: UIViewController {
    
    var lightOn = true
    
    override func viewDidLoad() {
        super.viewDidLoad()
        updateUI()
    }
    
    @IBAction func buttonPressed(_ sender: UIButton) {
        lightOn = !lightOn
        updateUI()
    }
    
    func updateUI() {
        view.backgroundColor = lightOn ? .white : .black
    }
    
    
    @IBOutlet var imageView: UIImageView!
    @IBAction func btnChange(_ sender: UIButton) {
        imageView.image = UIImage(named: "second")
    }
    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }
    
    
}


