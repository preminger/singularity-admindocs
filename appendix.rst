.. _installed-files:

#################
 Installed Files
#################

An installation of {Singularity} {InstallationVersion}, performed as
root via ``sudo make install`` consists of the following files, with
ownership and permissions required to use the `setuid` workflow:

.. code::

   # Main executables
   bin root:root 755 (drwxr-xr-x)
   bin/singularity root:root 755 (-rwxr-xr-x)
   bin/run-singularity root:root 755 (-rwxr-xr-x)

   # Configuration files
   etc root:root 755 (drwxr-xr-x)
   etc/bash_completion.d root:root 755 (drwxr-xr-x)
   etc/bash_completion.d/singularity root:root 644 (-rw-r--r--)
   etc/singularity root:root 755 (drwxr-xr-x)
   etc/singularity/singularity.conf root:root 644 (-rw-r--r--)
   etc/singularity/remote.yaml root:root 644 (-rw-r--r--)
   etc/singularity/network root:root 755 (drwxr-xr-x)
   etc/singularity/network/00_bridge.conflist root:root 644 (-rw-r--r--)
   etc/singularity/network/10_ptp.conflist root:root 644 (-rw-r--r--)
   etc/singularity/network/20_ipvlan.conflist root:root 644 (-rw-r--r--)
   etc/singularity/network/30_macvlan.conflist root:root 644 (-rw-r--r--)
   etc/singularity/network/40_fakeroot.conflist root:root 644 (-rw-r--r--)
   etc/singularity/capability.json root:root 644 (-rw-r--r--)
   etc/singularity/ecl.toml root:root 644 (-rw-r--r--)
   etc/singularity/seccomp-profiles root:root 755 (drwxr-xr-x)
   etc/singularity/seccomp-profiles/default.json root:root 644 (-rw-r--r--)
   etc/singularity/nvliblist.conf root:root 644 (-rw-r--r--)
   etc/singularity/rocmliblist.conf root:root 644 (-rw-r--r--)
   etc/singularity/cgroups root:root 755 (drwxr-xr-x)
   etc/singularity/cgroups/cgroups.toml root:root 644 (-rw-r--r--)
   etc/singularity/global-pgp-public root:root 644 (-rw-r--r--)

   # Runtime executables
   libexec root:root 755 (drwxr-xr-x)
   libexec/singularity root:root 755 (drwxr-xr-x)
   libexec/singularity/bin root:root 755 (drwxr-xr-x)
   libexec/singularity/bin/conmon root:root 755 (-rwxr-xr-x)
   libexec/singularity/bin/squashfuse_ll root:root 755 (-rwxr-xr-x)
   libexec/singularity/bin/starter root:root 755 (-rwxr-xr-x)
   libexec/singularity/bin/starter-suid root:root 4755 (-rwsr-xr-x)

   # CNI network plugins
   libexec/singularity/cni root:root 755 (drwxr-xr-x)
   libexec/singularity/cni/bandwidth root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/bridge root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/dhcp root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/firewall root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/host-device root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/host-local root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/ipvlan root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/loopback root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/macvlan root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/portmap root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/ptp root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/sbr root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/static root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/tap root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/tuning root:root 755 (-rwxr-xr-x)
   libexec/singularity/cni/vlan root:root 755 (-rwxr-xr-x) 
   libexec/singularity/cni/vrf root:root 755 (-rwxr-xr-x)

   # Documentation (man pages)
   share root:root 755 (drwxr-xr-x)
   share/man root:root 755 (drwxr-xr-x)
   share/man/man1 root:root 755 (drwxr-xr-x)
   share/man/man1/singularity.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-build.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-cache.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-cache-clean.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-cache-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-capability.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-capability-add.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-capability-avail.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-capability-drop.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-capability-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-config.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-config-fakeroot.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-config-global.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-delete.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-exec.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-inspect.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-instance.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-instance-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-instance-start.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-instance-stats.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-instance-stop.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key-export.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key-import.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key-newpair.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key-pull.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key-push.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key-remove.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-key-search.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-keyserver.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-keyserver-add.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-keyserver-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-keyserver-login.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-keyserver-logout.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-keyserver-remove.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-attach.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-create.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-delete.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-exec.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-kill.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-mount.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-pause.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-resume.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-run.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-start.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-state.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-umount.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-oci-update.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-overlay.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-overlay-create.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin-compile.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin-create.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin-disable.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin-enable.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin-inspect.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin-install.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-plugin-uninstall.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-pull.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-push.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-registry.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-registry-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-registry-login.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-registry-logout.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote-add.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote-get-login-password.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote-login.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote-logout.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote-remove.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote-status.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-remote-use.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-run.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-run-help.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-search.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-shell.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif-add.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif-del.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif-dump.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif-header.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif-info.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif-list.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif-new.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sif-setprim.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-sign.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-test.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-verify.1 root:root 644 (-rw-r--r--)
   share/man/man1/singularity-version.1 root:root 644 (-rw-r--r--)

   # Container state directories
   var root:root 755 (drwxr-xr-x)
   var/singularity root:root 755 (drwxr-xr-x)
   var/singularity/mnt root:root 755 (drwxr-xr-x)
   var/singularity/mnt/session root:root 755 (drwxr-xr-x)