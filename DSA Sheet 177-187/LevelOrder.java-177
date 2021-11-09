class Solution {
    public List<List<Integer>> levelOrder(TreeNode root) 
    {
        List<List<Integer>> solution=new ArrayList();
        ArrayList<Integer> list=new ArrayList<>();
        Queue<TreeNode> queue=new LinkedList<>();
        if(root==null)return Collections.emptyList();
        queue.add(root);
        queue.add(null);
        while(queue.size()!=1)
        {
            TreeNode front=queue.poll();
            if(front!=null)
            {
                list.add(front.val);
                if(front.left!=null)
                    queue.add(front.left);
                if(front.right!=null)
                    queue.add(front.right);
            }
            else
            {
                solution.add(list);
                list=new ArrayList<>();
                queue.add(null);
            }
        }
        solution.add(list);
        return solution;
    }
}
