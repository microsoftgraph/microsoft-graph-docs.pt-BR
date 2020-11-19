---
title: tipo de enumeração windowsDefenderProductStatus
description: Status do produto do Windows Defender
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0485dd4b375206d08ba0c744d0b0c3fca09b12c0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241136"
---
# <a name="windowsdefenderproductstatus-enum-type"></a>tipo de enumeração windowsDefenderProductStatus

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do produto do Windows Defender

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|NOSTATUS|,0|Sem status|
|serviceNotRunning|1|O serviço não está em execução|
|serviceStartedWithoutMalwareProtection|duas|Serviço iniciado sem qualquer mecanismo de proteção contra malware|
|pendingFullScanDueToThreatAction|4 |Verificação completa pendente devido à ação da ameaça|
|pendingRebootDueToThreatAction|8 |Reinicialização pendente devido à ação da ameaça|
|pendingManualStepsDueToThreatAction|16 |Etapas manuais pendentes devido à ação da ameaça |
|avSignaturesOutOfDate|32|Assinaturas AV desatualizadas|
|asSignaturesOutOfDate|64|COMO assinaturas desatualizadas|
|noQuickScanHappenedForSpecifiedPeriod|128|Nenhuma verificação rápida ocorreu por um período especificado|
|noFullScanHappenedForSpecifiedPeriod|256|Nenhuma verificação completa aconteceu por um período especificado|
|systemInitiatedScanInProgress|512|Verificação iniciada pelo sistema em andamento|
|systemInitiatedCleanInProgress|1024|O sistema iniciou a limpeza em andamento|
|samplesPendingSubmission|2048|Há amostras pendentes de envio|
|productRunningInEvaluationMode|4096|Produto em execução no modo de avaliação|
|productRunningInNonGenuineMode|8192|Produto executado em modo não original do Windows|
|productExpired|16384|Produto expirado|
|offlineScanRequired|32768|Varredura off-line obrigatória|
|serviceShutdownAsPartOfSystemShutdown|65536|O serviço está sendo desligado como parte do desligamento do sistema|
|threatRemediationFailedCritically|131072|A correção de ameaças falhou criticamente|
|threatRemediationFailedNonCritically|262144|Falha de correção de ameaça não crucial|
|noStatusFlagsSet|524288|Nenhum sinalizador de status definido (estado bem inicializado)|
|platformOutOfDate|1048576|A plataforma está desatualizada|
|platformUpdateInProgress|2097152|Atualização de plataforma em andamento|
|platformAboutToBeOutdated|4194304|A plataforma está prestes a ser desatualizada|
|signatureOrPlatformEndOfLifeIsPastOrIsImpending|8388608|A assinatura ou o fim da vida útil da plataforma está passado ou não está pendente|
|windowsSModeSignaturesInUseOnNonWin10SInstall|16777216|Assinaturas do Windows SMode ainda em uso na instalação não Win10S|




