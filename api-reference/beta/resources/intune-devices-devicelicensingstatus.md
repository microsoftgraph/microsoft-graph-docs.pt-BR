---
title: Tipo de enumeração deviceLicensingStatus
description: Indica o status de licenciamento do dispositivo depois que a assinatura baseada em dispositivo Windows foi habilitada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c0ff1ff53acd502fc6c92923b0a80a99e039d280
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671549"
---
# <a name="devicelicensingstatus-enum-type"></a>Tipo de enumeração deviceLicensingStatus

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o status de licenciamento do dispositivo depois que a assinatura baseada em dispositivo Windows foi habilitada.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|licenseRefreshStarted|0|Esse status é definido quando a atualização da licença é iniciada.|
|licenseRefreshPending|1|Esse status é definido quando a atualização da licença está pendente.|
|deviceIsNotAzureActiveDirectoryJoined|2|Esse status é definido quando o dispositivo não é ingressado no Azure Active Directory.|
|verifyingMicrosoftDeviceIdentity|3|Esse status é definido quando a identidade do dispositivo Microsoft está sendo verificada.|
|deviceIdentityVerificationFailed|4|Esse status é definido quando a verificação de identidade do dispositivo microsoft falha.|
|verifyingMirosoftAccountIdentity|5|Esse status é definido quando a identidade da conta da Microsoft está sendo verificada.|
|mirosoftAccountVerificationFailed|6 |Esse status é definido quando a verificação de identidade da conta da Microsoft falha.|
|acquiringDeviceLicense|7 |Esse status é definido quando a licença do dispositivo está sendo adquirida.|
|refreshingDeviceLicense|8 |Esse status é definido quando a licença do dispositivo está sendo atualizada.|
|deviceLicenseRefreshSucceed|9 |Esse status é definido quando a atualização da licença do dispositivo é bem-sucedida.|
|deviceLicenseRefreshFailed|10|Esse status é definido quando a atualização da licença do dispositivo falha.|
|removendoDeviceLicense|11|Esse status é definido quando a licença do dispositivo está sendo removida.|
|deviceLicenseRemoveSucceed|12 |Esse status é definido quando a remoção da licença do dispositivo é bem-sucedida.|
|deviceLicenseRemoveFailed|13|Esse status é definido quando a remoção da licença do dispositivo falha.|
|unknownFutureValue|14|Isso é colocado aqui como um espaço reservado para extensão futura.|
|desconhecido|-1|Padrão. Definido como desconhecido quando o status não pode ser determinado.|




