---
title: Tipo de recurso iosSingleSignOnSettings
description: Configurações de autenticação Kerberos do iOS para o login único
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 828117ad95c9e1de2815046d6877f5378528f788
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58804523"
---
# <a name="iossinglesignonsettings-resource-type"></a>Tipo de recurso iosSingleSignOnSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configurações de autenticação Kerberos do iOS para o login único

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAppsList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de identificadores de aplicativo que têm permissão para usar esse logon. Se esse campo for omitido, o logon se aplicará a todos os aplicativos no dispositivo. Esta coleção pode conter um máximo de 500 elementos.|
|allowedUrls|Coleção de cadeias de caracteres|Lista de URLs HTTP que devem ser corresponder para usar esse logon. Com o iOS 9.0 ou posterior, um caractere curinga pode ser usado.|
|displayName|Cadeia de caracteres|O nome de exibição das configurações de logon mostradas no dispositivo de recebimento.|
|kerberosPrincipalName|Cadeia de caracteres|Um nome principal Kerberos. Se não for fornecido, o usuário será solicitado a um durante a instalação do perfil.|
|kerberosRealm|Cadeia de caracteres|Um nome de domínio Kerberos. Case sensitive.|

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



