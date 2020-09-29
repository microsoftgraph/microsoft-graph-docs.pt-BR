---
title: Personalizar o cartão de perfil usando a API de perfil no Microsoft Graph (visualização)
description: Este artigo descreve como você pode personalizar o cartão de perfil tornando visíveis atributos adicionais ou adicionando atributos personalizados.
author: PollyNincevic
localization_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 5df48bc8da848c6e5655467ad9ef39a8bb992026
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288781"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-card-api-in-microsoft-graph-preview"></a><span data-ttu-id="aa270-103">Adicionar propriedades adicionais ao cartão de perfil usando a API do cartão de perfil no Microsoft Graph (visualização)</span><span class="sxs-lookup"><span data-stu-id="aa270-103">Add additional properties to the profile card using the profile card API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="aa270-104">No [cartão de perfil](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) no Microsoft 365, você pode encontrar informações sobre os usuários armazenados e mantidos pela sua organização, por exemplo **Título do cargo** ou **Local do escritório**.</span><span class="sxs-lookup"><span data-stu-id="aa270-104">On the [profile card](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) in Microsoft 365, you can find information about users that is stored and maintained by your organization, for example **Job title** or **Office location**.</span></span>

<span data-ttu-id="aa270-105">Use o recurso [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) para mostrar propriedades adicionais do Microsoft Azure Active Directory em cartões de perfil de uma organização:</span><span class="sxs-lookup"><span data-stu-id="aa270-105">Use the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource to show additional properties from Azure AD on profile cards for an organization, by:</span></span>

- <span data-ttu-id="aa270-106">Tornando visíveis atributos adicionais</span><span class="sxs-lookup"><span data-stu-id="aa270-106">Making additional attributes visible</span></span>

- <span data-ttu-id="aa270-107">Adicionando atributos personalizados</span><span class="sxs-lookup"><span data-stu-id="aa270-107">Adding custom attributes</span></span>

<span data-ttu-id="aa270-108">As propriedades adicionais serão exibidas na seção **Contato** do cartão de perfil no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="aa270-108">Additional properties will display in the **Contact** section of the profile card in Microsoft 365.</span></span>

> [!NOTE]
><span data-ttu-id="aa270-109">Operações no recurso **profileCardProperty** que usam permissões delegadas exigem que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="aa270-109">Operations on the **profileCardProperty** resource that use delegated permissions requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="make-additional-attributes-visible"></a><span data-ttu-id="aa270-110">Torne visíveis atributos adicionais</span><span class="sxs-lookup"><span data-stu-id="aa270-110">Make additional attributes visible</span></span>

<span data-ttu-id="aa270-111">Você pode fazer os seguintes atributos do Azure Active Directory (Azure AD) visíveis nos cartões de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="aa270-111">You can make the following attributes from Azure Active Directory (Azure AD) visible on users' profile cards.</span></span> <span data-ttu-id="aa270-112">Esses atributos *não diferenciam maiúsculas de minúsculas*:</span><span class="sxs-lookup"><span data-stu-id="aa270-112">These attributes are *not case-sensitive*:</span></span>

- `UserPrincipalName`
- `Fax`
- `StreetAddress`
- `PostalCode`
- `StateOrProvince`
- `Alias`

<span data-ttu-id="aa270-113">A tabela a seguir mostra como os atributos do Azure AD correspondem com as propriedades da entidade [user](/graph/api/resources/user?view=graph-rest-beta) do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aa270-113">The following table shows how the Azure AD attributes correspond with properties of the Microsoft Graph [user](/graph/api/resources/user?view=graph-rest-beta) entity.</span></span>

|<span data-ttu-id="aa270-114">Atributo do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="aa270-114">Azure AD attribute</span></span> |<span data-ttu-id="aa270-115">Propriedade da entidade User</span><span class="sxs-lookup"><span data-stu-id="aa270-115">User entity property</span></span>|
|:---------------|:----------|
|<span data-ttu-id="aa270-116">UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aa270-116">UserPrincipalName</span></span>|<span data-ttu-id="aa270-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aa270-117">userPrincipalName</span></span> |
|<span data-ttu-id="aa270-118">Fax</span><span class="sxs-lookup"><span data-stu-id="aa270-118">Fax</span></span>|<span data-ttu-id="aa270-119">faxNumber</span><span class="sxs-lookup"><span data-stu-id="aa270-119">faxNumber</span></span>|
|<span data-ttu-id="aa270-120">StreetAddress</span><span class="sxs-lookup"><span data-stu-id="aa270-120">StreetAddress</span></span>|<span data-ttu-id="aa270-121">streetAddress</span><span class="sxs-lookup"><span data-stu-id="aa270-121">streetAddress</span></span>|
|<span data-ttu-id="aa270-122">PostalCode</span><span class="sxs-lookup"><span data-stu-id="aa270-122">PostalCode</span></span>|<span data-ttu-id="aa270-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="aa270-123">postalCode</span></span>|
|<span data-ttu-id="aa270-124">StateOrProvince</span><span class="sxs-lookup"><span data-stu-id="aa270-124">StateOrProvince</span></span>|<span data-ttu-id="aa270-125">estado</span><span class="sxs-lookup"><span data-stu-id="aa270-125">state</span></span>
|<span data-ttu-id="aa270-126">Alias</span><span class="sxs-lookup"><span data-stu-id="aa270-126">Alias</span></span>|<span data-ttu-id="aa270-127">mailNickname</span><span class="sxs-lookup"><span data-stu-id="aa270-127">mailNickname</span></span>

<span data-ttu-id="aa270-128">Você pode adicionar qualquer um desses atributos ao cartão de perfil, configurando as [configurações da organização](/graph/api/resources/organizationsettings?view=graph-rest-beta) e adicionando o atributo como a propriedade *directoryPropertyName*\* de um **profileCardProperty** no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aa270-128">You can add any of these attributes to the profile card by configuring your [organization settings](/graph/api/resources/organizationsettings?view=graph-rest-beta) and adding the attribute as the *directoryPropertyName*\* property of a **profileCardProperty** in Microsoft Graph.</span></span> <span data-ttu-id="aa270-129">Ao tornar visíveis atributos adicionais, você deve usar os nomes de propriedades para `en-us`.</span><span class="sxs-lookup"><span data-stu-id="aa270-129">When you make additional attributes visible, you must use the property names for `en-us`.</span></span> <span data-ttu-id="aa270-130">Não é necessário adicionar valores localizados.</span><span class="sxs-lookup"><span data-stu-id="aa270-130">You don't have to add localized values.</span></span> <span data-ttu-id="aa270-131">As propriedades adicionais serão exibidas automaticamente nas configurações de idioma especificadas para o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="aa270-131">The additional properties will automatically be shown in the language settings that the user has specified for Microsoft 365.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="aa270-132">Ao adicionar um atributo ao cartão de perfil, leva até 24 horas para que a adição seja exibida.</span><span class="sxs-lookup"><span data-stu-id="aa270-132">When adding an attribute to profile card, it takes up to 24 hours for the addition to be displayed.</span></span>

## <a name="example"></a><span data-ttu-id="aa270-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa270-133">Example</span></span>

<span data-ttu-id="aa270-134">O exemplo a seguir exibe o atributo `Alias` no cartão de perfil:</span><span class="sxs-lookup"><span data-stu-id="aa270-134">The following example displays the `Alias` attribute on the profile card:</span></span>

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

<span data-ttu-id="aa270-135">Se bem-sucedido, este método retorna um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa270-135">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="aa270-136">O valor do atributo `Alias` seria exibido no cartão de perfil de um usuário.</span><span class="sxs-lookup"><span data-stu-id="aa270-136">The value for the `Alias` attribute  would be displayed on a user's profile card.</span></span>  

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a><span data-ttu-id="aa270-137">Adicionando atributos personalizados</span><span class="sxs-lookup"><span data-stu-id="aa270-137">Adding custom attributes</span></span>

<span data-ttu-id="aa270-138">Você pode adicionar qualquer um dos 15 [atributos de extensão personalizada](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) do Azure AD aos cartões de perfil do usuário, definindo as configurações da sua organização e [adicionando o valor correspondente como um profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aa270-138">You can add any of the 15 Azure AD [custom extension attributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) to users' profile cards by configuring your organization settings and [adding the corresponding value as a profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) in Microsoft Graph.</span></span> <span data-ttu-id="aa270-139">Você pode adicionar um recurso **profileCardProperty** por vez.</span><span class="sxs-lookup"><span data-stu-id="aa270-139">You can add one **profileCardProperty** resource at a time.</span></span>

<span data-ttu-id="aa270-140">São necessárias até 24 horas para que as alterações sejam mostradas em cartões de perfil.</span><span class="sxs-lookup"><span data-stu-id="aa270-140">It takes up to 24 hours for the changes to show on profile cards.</span></span>

<span data-ttu-id="aa270-141">As propriedades personalizadas não podem ser pesquisadas e não podem ser usadas para pesquisar pessoas em serviços e aplicativos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="aa270-141">Custom properties are not searchable and can't be used to search for people across Microsoft apps and services.</span></span>

<span data-ttu-id="aa270-142">A tabela a seguir mostra como os nomes de atributos de extensão personalizada do Microsoft Azure Active Directory correspondem aos valores com suporte para a propriedade **directoryPropertyName** do recurso [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="aa270-142">The following table shows how the Azure AD custom extension attribute names correspond to the supported values for the **directoryPropertyName** property of the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource.</span></span> <span data-ttu-id="aa270-143">Esses nomes de atributos de extensão personalizada do Microsoft Azure Active Directory *não fazem distinção entre maiúsculas e minúsculas*:</span><span class="sxs-lookup"><span data-stu-id="aa270-143">These Azure AD custom extension attribute names are *not case-sensitive*:</span></span>

|<span data-ttu-id="aa270-144">Atributo de extensão personalizada do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="aa270-144">Azure AD custom extension attribute</span></span> | <span data-ttu-id="aa270-145">Valor para especificar como directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="aa270-145">Value to specify as directoryPropertyName</span></span> |
|:--------------------|:-----------------|
| <span data-ttu-id="aa270-146">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="aa270-146">extensionAttribute1</span></span> | <span data-ttu-id="aa270-147">customAttribute1</span><span class="sxs-lookup"><span data-stu-id="aa270-147">customAttribute1</span></span> |
| <span data-ttu-id="aa270-148">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="aa270-148">extensionAttribute2</span></span> | <span data-ttu-id="aa270-149">customAttribute2</span><span class="sxs-lookup"><span data-stu-id="aa270-149">customAttribute2</span></span> |
| <span data-ttu-id="aa270-150">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="aa270-150">extensionAttribute3</span></span> | <span data-ttu-id="aa270-151">customAttribute3</span><span class="sxs-lookup"><span data-stu-id="aa270-151">customAttribute3</span></span> |
| <span data-ttu-id="aa270-152">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="aa270-152">extensionAttribute4</span></span> | <span data-ttu-id="aa270-153">customAttribute4</span><span class="sxs-lookup"><span data-stu-id="aa270-153">customAttribute4</span></span> |
| <span data-ttu-id="aa270-154">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="aa270-154">extensionAttribute5</span></span> | <span data-ttu-id="aa270-155">customAttribute5</span><span class="sxs-lookup"><span data-stu-id="aa270-155">customAttribute5</span></span> |
| <span data-ttu-id="aa270-156">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="aa270-156">extensionAttribute6</span></span> | <span data-ttu-id="aa270-157">customAttribute6</span><span class="sxs-lookup"><span data-stu-id="aa270-157">customAttribute6</span></span> |
| <span data-ttu-id="aa270-158">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="aa270-158">extensionAttribute7</span></span> | <span data-ttu-id="aa270-159">customAttribute7</span><span class="sxs-lookup"><span data-stu-id="aa270-159">customAttribute7</span></span> |
| <span data-ttu-id="aa270-160">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="aa270-160">extensionAttribute8</span></span> | <span data-ttu-id="aa270-161">customAttribute8</span><span class="sxs-lookup"><span data-stu-id="aa270-161">customAttribute8</span></span> |
| <span data-ttu-id="aa270-162">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="aa270-162">extensionAttribute9</span></span> | <span data-ttu-id="aa270-163">customAttribute9</span><span class="sxs-lookup"><span data-stu-id="aa270-163">customAttribute9</span></span> |
| <span data-ttu-id="aa270-164">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="aa270-164">extensionAttribute10</span></span> | <span data-ttu-id="aa270-165">customAttribute10</span><span class="sxs-lookup"><span data-stu-id="aa270-165">customAttribute10</span></span> |
| <span data-ttu-id="aa270-166">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="aa270-166">extensionAttribute11</span></span> | <span data-ttu-id="aa270-167">customAttribute11</span><span class="sxs-lookup"><span data-stu-id="aa270-167">customAttribute11</span></span> |
| <span data-ttu-id="aa270-168">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="aa270-168">extensionAttribute12</span></span> | <span data-ttu-id="aa270-169">customAttribute12</span><span class="sxs-lookup"><span data-stu-id="aa270-169">customAttribute12</span></span> |
| <span data-ttu-id="aa270-170">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="aa270-170">extensionAttribute13</span></span> | <span data-ttu-id="aa270-171">customAttribute13</span><span class="sxs-lookup"><span data-stu-id="aa270-171">customAttribute13</span></span> |
| <span data-ttu-id="aa270-172">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="aa270-172">extensionAttribute14</span></span> | <span data-ttu-id="aa270-173">customAttribute14</span><span class="sxs-lookup"><span data-stu-id="aa270-173">customAttribute14</span></span> |
| <span data-ttu-id="aa270-174">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="aa270-174">extensionAttribute15</span></span> | <span data-ttu-id="aa270-175">customAttribute15</span><span class="sxs-lookup"><span data-stu-id="aa270-175">customAttribute15</span></span> |

## <a name="example"></a><span data-ttu-id="aa270-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa270-176">Example</span></span>

<span data-ttu-id="aa270-177">O exemplo a seguir adiciona o primeiro atributo de extensão personalizada do Microsoft Azure Active Directory para o cartão de perfil, usando o nome de exibição **Centro de custos**.</span><span class="sxs-lookup"><span data-stu-id="aa270-177">The following example adds the first Azure AD custom extension attribute to the profile card, using the display name **Cost center**.</span></span> <span data-ttu-id="aa270-178">Para os usuários que definiram as configurações de idioma para o alemão, o nome de exibição será **Kostenstelle**.</span><span class="sxs-lookup"><span data-stu-id="aa270-178">For users that have set their language settings to German, the display name will be **Kostenstelle**.</span></span>

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

<span data-ttu-id="aa270-179">Se não houver suporte a um idioma, o nome da propriedade será mostrado com o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="aa270-179">If a language is not supported, the property name will be shown with the default value.</span></span>  

<span data-ttu-id="aa270-180">Se bem-sucedido, este método retorna um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa270-180">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="aa270-181">Neste exemplo, você pode supor que o cartão de perfil exiba **Kostenstelle** para todos os usuários que definiram as configurações de idioma para o alemão no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="aa270-181">In this example you can assume that the profile card displays **Kostenstelle** for all users that have set their language settings to German on the profile card.</span></span> <span data-ttu-id="aa270-182">Para todos os outros usuários, **Centro de custos** será exibido no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="aa270-182">For all other users, **Cost center** will be displayed on the profile card.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="aa270-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="aa270-183">See also</span></span>

[<span data-ttu-id="aa270-184">Localizar sua ID de locatário do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="aa270-184">Find your Microsoft 365 tenant ID</span></span>](/onedrive/find-your-office-365-tenant-id)

[<span data-ttu-id="aa270-185">Tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="aa270-185">onPremisesExtensionAttributes resource type</span></span>](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)

[<span data-ttu-id="aa270-186">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="aa270-186">User resource type</span></span>](/graph/api/resources/user?view=graph-rest-beta)

[<span data-ttu-id="aa270-187">Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="aa270-187">Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer)

[<span data-ttu-id="aa270-188">Obter profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="aa270-188">Get profileCardProperty</span></span>](/graph/api/profilecardproperty-get?view=graph-rest-beta)