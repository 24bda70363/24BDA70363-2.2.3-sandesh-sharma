# 24BDA70363-2.2.3-sandesh-sharma
Node* inorderSuccessor(Node* root, Node* x) {
    Node* successor = nullptr;

    while (root != nullptr) {
        if (x->data < root->data) {
            successor = root;
            root = root->left;
        } 
        else {
            root = root->right;
        }
    }

    return successor;
}
