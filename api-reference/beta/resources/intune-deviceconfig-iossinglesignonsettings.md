---
title: Tipo de recurso iosSingleSignOnSettings
description: Configurações de autenticação Kerberos do iOS para o login único
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f3d6ba266287e087ac9464ac99bc90d1505bb53
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59131326"
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
|allowedUrls|Conjunto de cadeias de caracteres|Lista de URLs HTTP que devem ser corresponder para usar esse logon. Com o iOS 9.0 ou posterior, um caractere curinga pode ser usado.|
|displayName|Cadeia de caracteres|O nome de exibição das configurações de logon mostradas no dispositivo de recebimento.|
|kerberosPrincipalName|Cadeia de Caracteres|Um nome principal Kerberos. Se não for fornecido, o usuário será solicitado a um durante a instalação do perfil.|
|kerberosRealm|Cadeia de Caracteres|Um nome de domínio Kerberos. Case sensitive.|

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



