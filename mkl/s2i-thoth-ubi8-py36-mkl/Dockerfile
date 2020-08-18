FROM quay.io/thoth-station/s2i-thoth-ubi8-py36

USER 0
RUN dnf config-manager --add-repo https://yum.repos.intel.com/setup/intelproducts.repo
RUN rpm --import https://yum.repos.intel.com/intel-gpg-keys/GPG-PUB-KEY-INTEL-SW-PRODUCTS-2019.PUB
RUN dnf install -y intel-mkl intel-ipp intel-tbb intel-daal intel-mpi intelpython3

USER 1042
