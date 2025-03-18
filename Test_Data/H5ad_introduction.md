{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 1,
   "id": "c4e40889-415f-4786-a0f9-6763b2cb38bb",
   "metadata": {
    "execution": {
     "iopub.execute_input": "2025-03-17T14:39:50.808891Z",
     "iopub.status.busy": "2025-03-17T14:39:50.808339Z",
     "iopub.status.idle": "2025-03-17T14:40:05.019978Z",
     "shell.execute_reply": "2025-03-17T14:40:05.018910Z",
     "shell.execute_reply.started": "2025-03-17T14:39:50.808847Z"
    }
   },
   "outputs": [],
   "source": [
    "import anndata as ad"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "id": "fee2fae0-323b-42ba-8ff1-929e98fe175d",
   "metadata": {
    "execution": {
     "iopub.execute_input": "2025-03-18T01:07:30.792847Z",
     "iopub.status.busy": "2025-03-18T01:07:30.792004Z",
     "iopub.status.idle": "2025-03-18T01:07:39.012690Z",
     "shell.execute_reply": "2025-03-18T01:07:39.011834Z",
     "shell.execute_reply.started": "2025-03-18T01:07:30.792770Z"
    }
   },
   "outputs": [],
   "source": [
    "adata = ad.read_h5ad(\"/data/users/guolongyu/SAW/test/rds_with_image/C04144D5.bin20_1.0.h5ad\")"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "id": "1ca368c5-5178-48fa-99fd-6fe8b58fe5f1",
   "metadata": {
    "execution": {
     "iopub.execute_input": "2025-03-18T01:07:39.013904Z",
     "iopub.status.busy": "2025-03-18T01:07:39.013697Z",
     "iopub.status.idle": "2025-03-18T01:07:39.020165Z",
     "shell.execute_reply": "2025-03-18T01:07:39.018729Z",
     "shell.execute_reply.started": "2025-03-18T01:07:39.013885Z"
    }
   },
   "outputs": [
    {
     "data": {
      "text/plain": [
       "AnnData object with n_obs × n_vars = 439383 × 29759\n",
       "    obs: 'total_counts', 'n_genes_by_counts', 'pct_counts_mt', 'leiden', 'orig.ident', 'x', 'y'\n",
       "    var: 'real_gene_name', 'n_cells', 'n_counts', 'mean_umi', 'means', 'dispersions', 'dispersions_norm', 'highly_variable'\n",
       "    uns: 'bin_size', 'bin_type', 'gene_exp_leiden', 'hvg', 'leiden_resolution', 'neighbors', 'omics', 'pca_variance_ratio', 'rank_genes_groups', 'resolution', 'sn'\n",
       "    obsm: 'X_pca', 'X_umap', 'spatial'\n",
       "    obsp: 'connectivities', 'distances'"
      ]
     },
     "execution_count": 6,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "adata"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "7212c90f-a9ba-496c-8950-2457caff3878",
   "metadata": {},
   "outputs": [],
   "source": [
    "adata.obs"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "stereopy-151",
   "language": "python",
   "name": "stereopy-151"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.8.20"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
