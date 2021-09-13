---
title: Tipo de número deviceManagementDomainJoinConnectorState
description: Os estados de solicitação ODJ.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cb637b2ee8d720859169dd10462334dde794de54
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017251"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a>Tipo de número deviceManagementDomainJoinConnectorState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Os estados de solicitação ODJ.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|active|0|O conector está pingando ativamente no Intune.|
|erro|1|Não há nenhuma batida do coração do conector da última hora.|
|inativo|2|Não há nenhuma batida do coração do conector dos últimos 5 dias.|



