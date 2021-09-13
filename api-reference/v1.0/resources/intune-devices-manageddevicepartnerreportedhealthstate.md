---
title: tipo denum managedDevicePartnerReportedHealthState
description: Estados de saúde disponíveis para a API de Saúde do Dispositivo
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c7ff45e140634c7683372628560a1fdb30efe446
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118219"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>tipo denum managedDevicePartnerReportedHealthState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados de saúde disponíveis para a API de Saúde do Dispositivo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O estado de saúde do dispositivo ainda não foi relatado|
|ativado|1|O dispositivo foi ativado por um parceiro de defesa contra ameaças móveis, mas ainda não relatou a saúde.|
|desativado|2|O dispositivo foi desativado por um parceiro de defesa contra ameaças móveis. A saúde do dispositivo não é conhecida.|
|secured|3|O dispositivo é considerado protegido pelo parceiro de defesa contra ameaças móveis.|
|lowSeverity|4 |O dispositivo é considerado baixa ameaça pelo parceiro de defesa contra ameaças móveis.|
|mediumSeverity|5 |O dispositivo é considerado uma ameaça média pelo parceiro de defesa contra ameaças móveis.|
|highSeverity|6 |O dispositivo é considerado alta ameaça pelo parceiro de defesa contra ameaças móveis.|
|não responsivo|7 |O dispositivo é considerado não responsivo pelo parceiro de defesa contra ameaças móveis. A saúde do dispositivo não é conhecida.|
|compromised|8 |O dispositivo é considerado comprometido pelo parceiro de Defesa contra Ameaças. Isso significa que o dispositivo tem uma Ameaça ou Risco ativo que não pode ser facilmente remediada pelo usuário final e o usuário deve entrar em contato com o administrador de IT.|
|misconfigured|9 |O dispositivo é considerado mal configurado com o parceiro de Defesa contra Ameaças. Isso significa que o dispositivo não tem um perfil ou configuração necessário para que o Parceiro de Defesa contra Ameaças funcione corretamente e, portanto, a análise de risco ou ameaça não é capaz de ser concluída.|




