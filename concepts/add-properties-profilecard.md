---
title: Personalizar o cartão de perfil usando a API de perfil no Microsoft Graph (visualização)
description: Este artigo descreve como você pode personalizar o cartão de perfil tornando mais atributos visíveis ou adicionando atributos personalizados.
author: PollyNincevic
localization_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: dc0c78ecfdf00488c7c9c12969eea8b405be496c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050971"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-api-in-microsoft-graph-preview"></a>Adicionar propriedades adicionais ao cartão de perfil usando a API de perfil no Microsoft Graph (visualização)

No [cartão de perfil](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) do Microsoft 365, você pode encontrar informações sobre os usuários que são armazenados e mantidos pela sua organização, por exemplo, **cargo** ou **local do escritório**.

Use o recurso [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) para mostrar propriedades adicionais do Azure AD em cartões de perfil para uma organização, por:

- Tornar mais atributos visíveis

- Adicionando atributos personalizados

Propriedades adicionais serão exibidas na seção **contato** do cartão de perfil no Microsoft 365.

> [!NOTE]
>As operações no recurso **profileCardProperty** que usam permissões delegadas exigem que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.

## <a name="make-additional-attributes-visible"></a>Tornar mais atributos visíveis

Você pode tornar os seguintes atributos do Azure Active Directory (Azure AD) visíveis nos cartões de perfil dos usuários. Esses atributos não diferenciam *maiúsculas de minúsculas*:

- `UserPrincipalName`
- `Fax`
- `StreetAddress`
- `PostalCode`
- `StateOrProvince`
- `Alias`

A tabela a seguir mostra como os atributos do Azure AD correspondem às propriedades da entidade de [usuário](/graph/api/resources/user?view=graph-rest-beta) do Microsoft Graph.

|Atributo do Azure AD |Propriedade da entidade User|
|:---------------|:----------|
|UserPrincipalName|userPrincipalName |
|Fax|faxNumber|
|StreetAddress|streetAddress|
|PostalCode|postalCode|
|StateOrProvince|estado
|Alias|mailNickname

Você pode adicionar qualquer um desses atributos ao cartão de perfil definindo suas [configurações da organização](/graph/api/resources/organizationsettings?view=graph-rest-beta) e adicionando o atributo como a propriedade *directoryPropertyName** de um **profileCardProperty** no Microsoft Graph. Ao tornar mais atributos visíveis, você deve usar os nomes de propriedade para `en-us` . Você não precisa adicionar valores localizados. As propriedades adicionais serão exibidas automaticamente nas configurações de idioma que o usuário especificou para o Microsoft 365.

> [!IMPORTANT]
> Ao adicionar um atributo ao cartão de perfil, leva até 24 horas para que a adição seja exibida.

## <a name="example"></a>Exemplo

O exemplo a seguir exibe o `Alias` atributo no cartão de perfil:

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

Se tiver êxito, a resposta retornará um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta. O valor do `Alias` atributo seria exibido no cartão de perfil de um usuário.  

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a>Adicionando atributos personalizados

Você pode adicionar qualquer um dos 15 atributos de [extensão personalizada](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) do Azure ad aos cartões de perfil dos usuários, definindo suas configurações de organização e [adicionando o valor correspondente como um ProfileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) no Microsoft Graph. Você pode adicionar um recurso **profileCardProperty** por vez.

É necessário até 24 horas para que as alterações sejam exibidas nos cartões de perfil.

As propriedades personalizadas não podem ser pesquisadas e não podem ser usadas para pesquisar pessoas em aplicativos e serviços da Microsoft.

A tabela a seguir mostra como os nomes de atributo de extensão personalizada do Azure AD correspondem aos valores com suporte para a propriedade **directoryPropertyName** do recurso [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) . Esses nomes de atributos de extensão personalizada do Azure AD não diferenciam *maiúsculas de minúsculas*:

|Atributo de extensão personalizada do Azure AD | Valor a ser especificado como directoryPropertyName |
|:--------------------|:-----------------|
| extensionAttribute1 | customAttribute1 |
| extensionAttribute2 | customAttribute2 |
| extensionAttribute3 | customAttribute3 |
| extensionAttribute4 | customAttribute4 |
| extensionAttribute5 | customAttribute5 |
| extensionAttribute6 | customAttribute6 |
| extensionAttribute7 | customAttribute7 |
| extensionAttribute8 | customAttribute8 |
| extensionAttribute9 | customAttribute9 |
| extensionAttribute10 | customAttribute10 |
| extensionAttribute11 | customAttribute11 |
| extensionAttribute12 | customAttribute12 |
| extensionAttribute13 | customAttribute13 |
| extensionAttribute14 | customAttribute14 |
| extensionAttribute15 | customAttribute15 |

## <a name="example"></a>Exemplo

O exemplo a seguir adiciona o primeiro atributo de extensão personalizado do Azure AD ao cartão de perfil, usando o nome de exibição **central de custos**. Para usuários que definiram suas configurações de idioma como alemão, o nome de exibição será **Kostenstelle**.

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

Se não houver suporte para um idioma, o nome da propriedade será mostrado com o valor padrão.  

Se tiver êxito, a resposta retornará um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta. Neste exemplo, você pode supor que o cartão de perfil exibe **Kostenstelle** para todos os usuários que definiram suas configurações de idioma como alemão no cartão de perfil. Para todos os outros usuários, o **centro de custos** será exibido no cartão de perfil.

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a>Confira também

[Encontre sua ID de locatário do Microsoft 365](https://docs.microsoft.com/onedrive/find-your-office-365-tenant-id)

[tipo de recurso Onpremisesextensionattributes à](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)

[Tipo de recurso de usuário](/graph/api/resources/user?view=graph-rest-beta)

[Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer)

[Obter profileCardProperty](/graph/api/profilecardproperty-get?view=graph-rest-beta)
