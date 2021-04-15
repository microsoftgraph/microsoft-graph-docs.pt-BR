---
title: Tipo de recurso teamsDeviceUsageUserDetail
description: Representa detalhes sobre o uso de dispositivos do Microsoft Teams pelo usuário.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 294ffee8a1a5db208508cce230377285d6834b07
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766053"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>Tipo de recurso teamsDeviceUsageUserDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes sobre o uso de dispositivos do Microsoft Teams pelo usuário.

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo    | Descrição                                                  |
| :---------------- | :------ | ------------------------------------------------------------ |
| reportRefreshDate | Data    | A data mais recente do conteúdo.                              |
| userPrincipalName | String  | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. |
| isLicensed        | Booliano | Se o usuário recebeu uma licença do Teams.          |
| lastActivityDate  | Data    | A última data em que o usuário participou de uma atividade do Microsoft Teams. |
| isDeleted         | Booliano | Se esse usuário foi excluído ou excluído.          |
| deletedDate       | Data    | A data em que a operação de exclusão aconteceu. O valor padrão é "null" quando o usuário não foi excluído. |
| usedWeb           | Booliano | Se o usuário estava ativo no cliente Web do Teams em dispositivos. |
| usedWindowsPhone  | Booliano | Se o usuário estava ativo no cliente móvel do Teams para o telefone Windows. |
| usediOS           | Booliano | Se o usuário estava ativo no cliente móvel do Teams para iOS. |
| usedMac           | Booliano | Se o usuário estava ativo no cliente de área de trabalho do Teams em um computador macOS. |
| usedAndroidPhone  | Booliano | Se o usuário estava ativo no cliente móvel do Teams para Android. |
| usedWindows       | Booliano | Se o usuário estava ativo no cliente de área de trabalho do Teams em um computador baseado no Windows. |
| usedChromeOS      | Booliano | Se o usuário estava ativo no cliente da área de trabalho do Teams em um computador ChromeOS. |
| usedLinux         | Booliano | Se o usuário estava ativo no cliente de área de trabalho do Teams em um computador Linux. |
| reportPeriod      | String  | O número de dias que o relatório aborda.                        |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "usedChromeOS": true, 
  "usedLinux": true, 
  "reportPeriod": "String"
}
```


