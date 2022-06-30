---
title: Adicionar ou excluir atributos personalizados em um cartão de perfil (versão prévia)
description: Saiba como usar a API de cartão de perfil no Microsoft Graph para deixar atributos adicionais visíveis e adicionar ou excluir atributos personalizados em um cartão de perfil.
author: PollyNincevic
ms.localizationpriority: high
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9d1685ef287cb7cea973b452a1b05d70b8d1d144
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441010"
---
# <a name="add-or-delete-custom-attributes-on-a-profile-card-using-the-profile-card-api-preview"></a>Adicionar ou excluir atributos personalizados em um cartão de perfil usando a API de cartão de perfil (versão prévia)

No cartão de perfil no Microsoft 365, você pode encontrar informações sobre os usuários armazenados e mantidos pela sua organização, por exemplo **Título do cargo** ou **Local do escritório**.

Use o recurso [profileCardProperty](/graph/api/resources/profilecardproperty) para mostrar propriedades adicionais do Microsoft Azure Active Directory em cartões de perfil de uma organização:

* Tornando visíveis atributos adicionais
* Adicionando atributos personalizados

As propriedades adicionais são exibidas na seção **Contato** do cartão de perfil no Microsoft 365.

Você também pode [excluir](/graph/api/profilecardproperty-delete?view=graph-rest-beta&preserve-view=true) atributos personalizados dos cartões de perfil da organização.

> [!NOTE]
> As operações no recurso **profileCardProperty** que usam permissões delegadas exigem que o usuário conectado tenha um administrador de locatários ou a função de administrador global.

## <a name="make-additional-attributes-visible"></a>Deixe os atributos adicionais visíveis

Você pode deixar os seguintes atributos do Azure Active Directory (Azure AD) visíveis nos cartões de perfil do usuário. Esses atributos não *diferenciam maiúsculas de minúsculas*:

* `UserPrincipalName`
* `Fax`
* `StreetAddress`
* `PostalCode`
* `StateOrProvince`
* `Alias`

A tabela a seguir mostra como os atributos do Azure AD correspondem com as propriedades da entidade [user](/graph/api/resources/user) do Microsoft Graph.

| Atributo do Microsoft Azure Active Directory | Propriedade da entidade User |
| ------------------ | -------------------- |
| UserPrincipalName | userPrincipalName |
| Fax | faxNumber |
| StreetAddress | streetAddress |
| PostalCode | postalCode |
| StateOrProvince | estado |
| Alias | mailNickname |

Você pode adicionar qualquer desses atributos ao cartão de perfil, configurando suas [configurações da organização](/graph/api/resources/organizationsettings) e adicionando o atributo como a propriedade **directoryPropertyName** de um **profileCardProperty** no Microsoft Graph. Ao tornar visíveis atributos adicionais, você deve usar os nomes de propriedades para `en-us`. Não é necessário adicionar valores localizados. As propriedades adicionais serão exibidas automaticamente nas configurações de idioma especificadas para o Microsoft 365.

> [!IMPORTANT]
> Ao adicionar um atributo ao cartão de perfil, leva até 24 horas para que a adição seja exibida.

### <a name="example"></a>Exemplo

O exemplo a seguir exibe o `Alias` atributo no cartão de perfil.

``` http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

Se bem-sucedido, esse método retorna um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta. O valor do `Alias` atributo será exibido no cartão de perfil de um usuário.

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="add-a-custom-attribute"></a>Adicionar um atributo personalizado

Você pode adicionar qualquer desses 15 [atributos de extensão personalizada](/graph/api/resources/onpremisesextensionattributes) do Azure AD aos cartões de perfil do usuário ao definir as configurações da sua organização e [ao adicionar o valor correspondente como um profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties) no Microsoft Graph. Você pode adicionar um recurso **profileCardProperty** de cada vez.

São necessárias até 24 horas para que as alterações sejam mostradas em cartões de perfil.

As propriedades personalizadas não podem ser pesquisadas e não podem ser usadas para pesquisar pessoas em serviços e aplicativos da Microsoft.

A tabela a seguir mostra como os nomes de atributo de extensão personalizada do Azure AD correspondem aos valores com suporte para a propriedade **directoryPropertyName** do recurso [profileCardProperty](/graph/api/resources/profilecardproperty). Esses nomes de atributo de extensão personalizada do Azure AD não diferenciam *maiúsculas de minúsculas*:

| Atributo de extensão personalizada do Microsoft Azure Active Directory | Valor para especificar como directoryPropertyName |
| ----------------------------------- | ----------------------------------------- |
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

### <a name="example"></a>Exemplo

O exemplo a seguir adiciona o primeiro atributo de extensão personalizada do Microsoft Azure Active Directory para o cartão de perfil, usando o nome de exibição **Centro de custos**. Para os usuários que definiram as configurações de idioma para o alemão, o nome de exibição será **Kostenstelle**.

#### <a name="request"></a>Solicitação

``` http
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

Se não houver suporte a um idioma, o nome da propriedade será mostrado com o valor padrão.

Se bem-sucedido, este método retorna um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta. Neste exemplo, você pode supor que o cartão de perfil exiba **Kostenstelle** para todos os usuários que definiram as configurações de idioma para o alemão no cartão de perfil. Para todos os outros usuários, **Centro de custos** será exibido no cartão de perfil.

#### <a name="response"></a>Resposta

``` http
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

## <a name="delete-a-custom-attribute"></a>Excluir um atributo personalizado

Seguindo o mesmo mapeamento entre atributos de extensão personalizada do Azure AD e atributos personalizados do cartão de perfil (como `customAttribute1`), conforme descrito na seção anterior [Adicionando um atributo personalizado](/graph/add-properties-profilecard#adding-a-custom-attribute), você pode excluir um atributo personalizado usando a operação de [exclusão](/graph/api/profilecardproperty-delete?view=graph-rest-beta&preserve-view=true), conforme mostrado no exemplo a seguir.

### <a name="example"></a>Exemplo

O exemplo a seguir exclui o atributo personalizado `customAttribute5` das configurações da organização. Uma exclusão bem-sucedida retorna `HTTP 204`.

#### <a name="request"></a>Solicitação

``` http
DELETE https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/customAttribute5
```

#### <a name="response"></a>Resposta

``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Confira também

- [Localizar sua ID de locatário do Microsoft 365](/onedrive/find-your-office-365-tenant-id)
- [Tipo de recurso onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes)
- [Tipo de recurso de usuário](/graph/api/resources/user)
- [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer)
- [Obter profileCardProperty](/graph/api/profilecardproperty-get)
