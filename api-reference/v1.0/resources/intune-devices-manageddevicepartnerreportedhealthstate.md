---
title: Tipo de enumeração managedDevicePartnerReportedHealthState
description: Estados de integridade disponíveis para a API de Integridade do Dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 775a8d6419b8370e7c962432780b5f0d2e3e0ae4
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66729955"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>Tipo de enumeração managedDevicePartnerReportedHealthState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados de integridade disponíveis para a API de Integridade do Dispositivo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O estado de integridade do dispositivo ainda não foi relatado|
|Ativado|1|O dispositivo foi ativado por um parceiro de defesa contra ameaças móveis, mas ainda não relatou a integridade.|
|Desativado|2|O dispositivo foi desativado por um parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|Seguro|3|O dispositivo é considerado protegido pelo parceiro de defesa contra ameaças móveis.|
|lowSeverity|4|O dispositivo é considerado uma ameaça baixa pelo parceiro de defesa contra ameaças móveis.|
|mediumSeverity|5|O dispositivo é considerado uma ameaça média pelo parceiro de defesa contra ameaças móveis.|
|highSeverity|6 |O dispositivo é considerado uma ameaça alta pelo parceiro de defesa contra ameaças móveis.|
|Responder|7 |O dispositivo é considerado sem resposta pelo parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|Comprometida|8 |O dispositivo é considerado comprometido pelo parceiro de Defesa contra Ameaças. Isso significa que o dispositivo tem uma Ameaça ou Risco ativa que não pode ser facilmente corrigida pelo usuário final e o usuário deve entrar em contato com a equipe de TI Administração.|
|Errada|9 |O dispositivo é considerado configurado incorretamente com o parceiro de Defesa contra Ameaças. Isso significa que o dispositivo não tem um perfil ou configuração necessário para que o Parceiro de Defesa contra Ameaças funcione corretamente e, portanto, a análise de risco ou ameaça não é capaz de ser concluída.|





