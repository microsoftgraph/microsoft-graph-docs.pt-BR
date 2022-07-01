---
title: Adicionar dados personalizados aos usuários usando extensões abertas
description: Siga as etapas deste exemplo para adicionar uma extensão, consultar um usuário e retornar um perfil móvel, alterar e depois excluir as informações do perfil móvel do usuário.
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: a94fd34daff722c0fd32bd271618626db1f50cec
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556189"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a>Adicionar dados personalizados aos usuários usando extensões abertas
Neste artigo você será guiado através de um exemplo para ilustrar o uso de *extensões abertas*. 

Imagine que você está criando um aplicativo que está disponível em várias plataformas cliente diferentes, como computadores e dispositivos móveis.  Você gostaria que os usuários pudessem configurar a própria experiência de interface do usuário para que ela fosse consistente, independentemente do dispositivo usado para entrar no seu aplicativo. Este é um requisito comum para a maioria dos aplicativos. 

Para este cenário, este artigo lhe mostrará como:

1. Adicionar uma extensão aberta representando algumas informações do perfil móvel sobre o usuário.
2. Consultar o usuário e retornar o perfil móvel.
3. Alterar as informações do perfil móvel do usuário (o valor de extensão aberta).
4. Excluir informações do perfil móvel do usuário.

> [!NOTE]
> Este tópico mostra como adicionar, ler, atualizar e excluir extensões abertas em um recurso do **usuário**. Extensões abertas também têm suporte e podem ser gerenciadas para [outros tipos de recursos](extensibility-overview.md).

## <a name="1-add-roaming-profile-information"></a>1. Adicionar informações de perfil móvel
O usuário entra no aplicativo e configura a aparência do aplicativo.  Essas configurações de aplicativo devem transitar para que o usuário obtenha a mesma experiência em praticamente qualquer dispositivo usado para entrar no aplicativo.  Aqui, veremos como adicionar as informações do perfil móvel a um recurso user.

### <a name="request"></a>Solicitação
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
### <a name="response"></a>Resposta
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a>2. Recuperar informações do perfil móvel do usuário.
Quando o usuário entra no aplicativo de outro dispositivo, o aplicativo pode recuperar detalhes do perfil do usuário, além das configurações de roaming dele. Isso pode ser feito obtendo recursos do usuário e expandindo a propriedade de navegação da extensão.

### <a name="request"></a>Solicitação
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
### <a name="response"></a>Resposta
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```

> [!NOTE]
> Se você tiver várias extensões, você pode filtrar na **ID** para obter a extensão que lhe interessa.

## <a name="3-change-roaming-profile-information"></a>3. Alterar informações de perfil móvel
O usuário pode escolher alterar as próprias informações do perfil móvel.  Esta atualização pode ser feita com um ```PATCH``` no valor da extensão aberta. 

### <a name="request"></a>Solicitação
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

### <a name="response"></a>Resposta
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a>4. Excluir um perfil de usuário móvel
O usuário decide que, se não quiser mais um perfil móvel, pode excluí-lo. Esta atualização pode ser feita com uma solicitação ```DELETE``` no valor extensão aberto.

### <a name="request"></a>Solicitação
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

### <a name="response"></a>Resposta
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](extensibility-overview.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](extensibility-schema-groups.md)
- [tipo de recurso openTypeExtension](/graph/api/resources/opentypeextension)
- [Criar extensão aberta](/graph/api/opentypeextension-post-opentypeextension)
- [Obter extensão aberta](/graph/api/opentypeextension-get)
- [Atualizar extensão aberta](/graph/api/opentypeextension-update)
- [Excluir extensão aberta](/graph/api/opentypeextension-delete)
