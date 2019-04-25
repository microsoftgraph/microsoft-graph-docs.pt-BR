---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a475f32d4572b0aa8ed2a52befc7a58eb6077253
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541162"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>tipo de enumeração firewallCertificateRevocationListCheckMethodType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|Nenhuma|1 |Não verificar a lista de certificados revogados|
|Houve|2 |Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação|
|precisa|3 |Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado|



