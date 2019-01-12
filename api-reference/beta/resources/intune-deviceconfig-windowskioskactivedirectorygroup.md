---
title: tipo de recurso de windowsKioskActiveDirectoryGroup
description: A classe usada para identificar um grupo de diretório do Windows Azure para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 632396b727448032f198a54b97ba0a46b961abe5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955230"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a>tipo de recurso de windowsKioskActiveDirectoryGroup

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A classe usada para identificar um grupo de diretório do Windows Azure para a configuração de quiosque

Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|groupName|Cadeia de caracteres|O nome do grupo AD que será bloqueado para esta configuração de quiosque|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





