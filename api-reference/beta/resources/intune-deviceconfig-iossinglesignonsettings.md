---
title: tipo de recurso iosSingleSignOnSettings
description: configurações de autenticação Kerberos do iOS para logon único
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5f35240243b94a2abdc817823b70d53a64b43dca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529857"
---
# <a name="iossinglesignonsettings-resource-type"></a>tipo de recurso iosSingleSignOnSettings

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

configurações de autenticação Kerberos do iOS para logon único

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAppsList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de identificadores de aplicativos que têm permissão para usar esse logon. Se esse campo for omitido, o logon será aplicado a todos os aplicativos no dispositivo. Esta coleção pode conter um máximo de 500 elementos.|
|allowedUrls|String collection|Lista de URLs HTTP que devem ser correspondidas para usar esse logon. Com o iOS 9,0 ou posterior, um caractere curinga pode ser usado.|
|displayName|String|O nome de exibição das configurações de logon mostradas no dispositivo receptor.|
|kerberosPrincipalName|String|Um nome principal Kerberos. Se não for fornecido, o usuário será solicitado a fornecer um durante a instalação do perfil.|
|kerberosRealm|String|Um nome de realm Kerberos. Diferencia maiúsculas de minúsculas.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```



