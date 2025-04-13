# CBT651
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE 651 is from Chip Grantham and contains MVS batch programs *   FILE 651
//*           which are designed to reset BWO flags.  Sample output *   FILE 651
//*           from this package, which really is in FBA, LRECL=133  *   FILE 651
//*           format, but which has been reformatted for packaging  *   FILE 651
//*           by the TSO XMIT command, is included here as member   *   FILE 651
//*           $OUTPUT.                                              *   FILE 651
//*                                                                 *   FILE 651
//*           email:  cgrantha@notes.state.ne.us                    *   FILE 651
//*                                                                 *   FILE 651
//*     Here is some text about the BWO flags, who cares, and       *   FILE 651
//*     what the program does:                                      *   FILE 651
//*                                                                 *   FILE 651
//*     DFSMSdss supports backup-while-open serialization, which    *   FILE 651
//*     can perform backup of data sets that are open for update    *   FILE 651
//*     for long periods of time.  It can also perform a logical    *   FILE 651
//*     data set dump of these data sets even if another            *   FILE 651
//*     application has them serialized.  Backup-while-open is a    *   FILE 651
//*     better method than using SHARE or TOLERATE(ENQFAILURE)      *   FILE 651
//*     for dumping CICS VSAM file-control data sets that are       *   FILE 651
//*     in-use and open for update.  When you dump data sets that   *   FILE 651
//*     are designated by CICS as eligible for backup-while-open    *   FILE 651
//*     processing, data integrity is maintained through            *   FILE 651
//*     serialization interactions between CICS (data base          *   FILE 651
//*     control program), CICSVR (forward-recovery program),        *   FILE 651
//*     VSAM record management, DFSMSdfp, and DFSMSdss.             *   FILE 651
//*                                                                 *   FILE 651
//*     Keywords from the IDCAMS Define, Current Catalog time       *   FILE 651
//*     and date stamps, and Backup-While-Open flags may need       *   FILE 651
//*     to be reviewed when performing a recovery or backup.        *   FILE 651
//*                                                                 *   FILE 651
//*     The program GDERLSBT will report on current status of       *   FILE 651
//*     these indicators from all sources.  The input may be a      *   FILE 651
//*     specific dataset or may be a catalog filter.                *   FILE 651
//*                                                                 *   FILE 651
//*     The input control statement                                 *   FILE 651
//*       SHOW=<dsname>                                             *   FILE 651
//*     will report on RLS indicators for the requested dsname.     *   FILE 651
//*     The input control statement                                 *   FILE 651
//*       LEVEL=<catalog filter>                                    *   FILE 651
//*     will search the master catalog and usercatalogs using       *   FILE 651
//*     IGGCSI00 for VSAM clusters reporting on every dataset       *   FILE 651
//*     which meet the filter qualifications.                       *   FILE 651
//*                                                                 *   FILE 651
//*     The program GDEBWOBT will facilitate the setting of the     *   FILE 651
//*     BWO control flags.  The setting of the flags may be         *   FILE 651
//*     required to accommodate backup-while-open processing,       *   FILE 651
//*     build testing scenarios, or allow processing by CICSVR      *   FILE 651
//*     and/or CICS.                                                *   FILE 651
//*                                                                 *   FILE 651
```
