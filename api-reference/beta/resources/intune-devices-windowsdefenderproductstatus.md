---
title: tipo de número windowsDefenderProductStatus
description: Status do produto Windows Defender
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 17a5854c2579a039012b31950cce8660f6031a8c3048e437ffc52e94f6a18f23
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122408"
---
# <a name="windowsdefenderproductstatus-enum-type"></a>tipo de número windowsDefenderProductStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do produto Windows Defender

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noStatus|0|Sem status|
|serviceNotRunning|1 |Serviço não em execução|
|serviceStartedWithoutMalwareProtection|2|Serviço iniciado sem qualquer mecanismo de proteção contra malware|
|pendingFullScanDueToThreatAction|4 |Verificação completa pendente devido à ação de ameaça|
|pendingRebootDueToThreatAction|8 |Reinicialização pendente devido à ação de ameaça|
|pendingManualStepsDueToThreatAction|16 |Etapas manuais pendentes devido à ação contra ameaças |
|avSignaturesOutOfDate|32|Assinaturas AV des date|
|asSignaturesOutOfDate|64|Assinaturas AS desa datadas|
|noQuickScanHappenedForSpecifiedPeriod|128|Nenhuma verificação rápida ocorreu por um período especificado|
|noFullScanHappenedForSpecifiedPeriod|256|Nenhuma verificação completa ocorreu por um período especificado|
|systemInitiatedScanInProgress|512|Verificação iniciada pelo sistema em andamento|
|systemInitiatedCleanInProgress|1024|Sistema iniciado limpo em andamento|
|samplesPendingSubmission|2048|Há exemplos pendentes de envio|
|productRunningInEvaluationMode|4096|Produto em execução no modo de avaliação|
|productRunningInNonGenuineMode|8192|Produto em execução no modo não Windows original|
|productExpired|16384|Produto expirado|
|offlineScanRequired|32768|Verificação off-line necessária|
|serviceShutdownAsPartOfSystemShutdown|65536|O serviço está sendo desligado como parte do desligamento do sistema|
|threatRemediationFailedCritically|131072|Falha crítica na correção de ameaças|
|threatRemediationFailedNonCritically|262144|A correção de ameaças falhou de forma não crítica|
|noStatusFlagsSet|524288|Nenhum conjunto de sinalizadores de status (estado bem inicializado)|
|platformOutOfDate|1048576|A plataforma está des date|
|platformUpdateInProgress|2097152|A atualização da plataforma está em andamento|
|platformAboutToBeOutdated|4194304|A plataforma está prestes a ficar desatualizada|
|signatureOrPlatformEndOfLifeIsPastOrIsImpending|8388608|A assinatura ou o fim da vida útil da plataforma é passado ou está pendente|
|windowsSModeSignaturesInUseOnNonWin10SInstall|16777216|Windows Assinaturas SMode ainda em uso na instalação não Win10S|




