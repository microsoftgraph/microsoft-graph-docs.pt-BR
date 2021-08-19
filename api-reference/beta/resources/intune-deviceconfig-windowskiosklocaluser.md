---
title: Tipo de recurso windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração de quiosque
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 69aba030afe0e918f4aab08a5e990e64846571fe57305a999350df2d8bc2ce8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139499"
---
# <a name="windowskiosklocaluser-resource-type"></a>Tipo de recurso windowsKioskLocalUser

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe usada para identificar uma conta local para a configuração de quiosque


Herda do [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userName|Cadeia de caracteres|O usuário local que será bloqueado para essa configuração de quiosque|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```




