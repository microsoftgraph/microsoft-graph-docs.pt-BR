---
title: tipo de recurso de windowsKioskAzureADUser
description: A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4497c6d42db45f518e3ef93e78e50d25f473ac00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984140"
---
# <a name="windowskioskazureaduser-resource-type"></a>tipo de recurso de windowsKioskAzureADUser

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A classe usada para identificar uma conta de usuário AzureAD para a configuração de quiosque

Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userId|Cadeia de caracteres|A ID do usuário AzureAD que será bloqueado para esta configuração de quiosque|
|userPrincipalName|Cadeia de caracteres|As contas de usuário que serão bloqueadas para esta configuração de quiosque|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```





