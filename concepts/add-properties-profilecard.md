---
title: Personalizar o cartão de perfil usando a API de perfil no Microsoft Graph (visualização)
description: Este artigo descreve como você pode personalizar o cartão de perfil tornando visíveis atributos adicionais ou adicionando atributos personalizados.
author: PollyNincevic
localization\_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 85ec4c8bd842b01f441ef6c34b2c7be288ec059d5a30f3d73ac796cdc64e76be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146326"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-card-api-in-microsoft-graph-preview"></a>Adicionar propriedades adicionais ao cartão de perfil usando a API do cartão de perfil no Microsoft Graph (visualização)

No [cartão de perfil](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) no Microsoft 365, você pode encontrar informações sobre os usuários armazenados e mantidos pela sua organização, por exemplo **Título do cargo** ou **Local do escritório**.

Use o recurso [profileCardProperty](/graph/api/resources/profilecardproperty) para mostrar propriedades adicionais do Microsoft Azure Active Directory em cartões de perfil de uma organização:

* Tornando visíveis atributos adicionais
* Adicionando atributos personalizados

As propriedades adicionais serão exibidas na seção **Contato** do cartão de perfil no Microsoft 365.

> [!NOTE]
> As operações no **recurso profileCardProperty** que usam permissões delegadas exigem que o usuário de entrada tenha um administrador de locatário ou uma função de administrador global.

## <a name="make-additional-attributes-visible"></a>Torne visíveis atributos adicionais

Você pode fazer os seguintes atributos do Azure Active Directory (Azure AD) visíveis nos cartões de perfil do usuário. Esses atributos *não diferenciam maiúsculas de minúsculas*:

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

Você pode adicionar qualquer um desses atributos ao [](/graph/api/resources/organizationsettings) cartão de perfil configurando as configurações da sua organização e adicionando o atributo como a **propriedade directoryPropertyName** de **um profileCardProperty** no Microsoft Graph. Ao tornar visíveis atributos adicionais, você deve usar os nomes de propriedades para `en-us`. Não é necessário adicionar valores localizados. As propriedades adicionais serão exibidas automaticamente nas configurações de idioma especificadas para o Microsoft 365.

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

Se bem-sucedido, este método retorna um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta. O valor do `Alias` atributo seria exibido no cartão de perfil de um usuário.

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a>Adicionando atributos personalizados

Você pode adicionar qualquer um dos 15 [atributos de extensão personalizada](/graph/api/resources/onpremisesextensionattributes) do Azure AD aos cartões de perfil do usuário, definindo as configurações da sua organização e [adicionando o valor correspondente como um profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties) no Microsoft Graph. Você pode adicionar um recurso **profileCardProperty** por vez.

São necessárias até 24 horas para que as alterações sejam mostradas em cartões de perfil.

As propriedades personalizadas não podem ser pesquisadas e não podem ser usadas para pesquisar pessoas em serviços e aplicativos da Microsoft.

A tabela a seguir mostra como os nomes de atributos de extensão personalizada do Microsoft Azure Active Directory correspondem aos valores com suporte para a propriedade **directoryPropertyName** do recurso [profileCardProperty](/graph/api/resources/profilecardproperty). Esses nomes de atributos de extensão personalizada do Microsoft Azure Active Directory *não fazem distinção entre maiúsculas e minúsculas*:

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

## <a name="see-also"></a>Confira também

- [Localizar sua ID de locatário do Microsoft 365](/onedrive/find-your-office-365-tenant-id)
- [Tipo de recurso onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes)
- [Tipo de recurso de usuário](/graph/api/resources/user)
- [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer)
- [Obter profileCardProperty](/graph/api/profilecardproperty-get)
