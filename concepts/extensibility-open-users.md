---
title: Adicionar dados personalizados aos usuários usando extensões abertas
description: 'Neste artigo você será guiado através de um exemplo para ilustrar o uso de *extensões abertas*. '
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 06acd010f9528aae12e768aadd4f8e9e62ace651
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143562"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a>Adicionar dados personalizados aos usuários usando extensões abertas
Neste artigo você será guiado através de um exemplo para ilustrar o uso de *extensões abertas*. 

Imagine que você está criando um aplicativo que está disponível em várias plataformas cliente diferentes, como computadores e dispositivos móveis.  Você gostaria que os usuários pudessem configurar a própria experiência de interface do usuário para que ela fosse consistente, independentemente do dispositivo usado para entrar no seu aplicativo. Este é um requisito comum para a maioria dos aplicativos. 

Para este cenário, este artigo lhe mostrará como:

1. Adicionar uma extensão aberta representando algumas informações do perfil móvel sobre o usuário.
2. Consultar o usuário e retornar o perfil móvel.
3. Alterar as informações do perfil móvel do usuário (o valor de extensão aberta).
4. Excluir informações do perfil móvel do usuário.

>**Observação:** Este tópico mostrará a você como adicionar, ler, atualizar e excluir extensões abertas em um recurso de **user**. Esses métodos também são suportados para os tipos de recurso **administrativeUnit**, **contact**, **device**, **event**, **group**, **organization**, **post**, **todoTask**, e **todoTaskList**.  
Você pode atualizar os exemplos de solicitação usando qualquer um desses tipos de recursos. As respostas ilustradas nos exemplos poderiam ser reduzidas para facilitar a leitura. 

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
Content-length: 420

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
Content-length: 420

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
>**Observação:** Se você tiver várias extensões, você pode filtrar na **id** para obter a extensão que lhe interessa.

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
- [tipo de recurso openTypeExtension](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [Criar extensão aberta](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [Obter extensão aberta](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [Atualizar extensão aberta](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [Excluir extensão aberta](/graph/api/opentypeextension-delete?view=graph-rest-1.0)
