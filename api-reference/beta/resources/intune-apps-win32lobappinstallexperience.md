---
title: Tipo de recurso win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo Win32
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 098f3dd9e240102bd6e48d345073eb0f3a090bd1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127532"
---
# <a name="win32lobappinstallexperience-resource-type"></a>Tipo de recurso win32LobAppInstallExperience

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de experiência de instalação para um aplicativo Win32

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução em que o aplicativo é executado. Os valores possíveis são: `system` e `user`.|
|deviceRestartBehavior|[win32LobAppRestartBehavior](../resources/intune-apps-win32lobapprestartbehavior.md)|Comportamento de reinicialização do dispositivo. Os valores possíveis são: `basedOnReturnCode`, `allow`, `suppress`, `force`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String",
  "deviceRestartBehavior": "String"
}
```



