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
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-api-in-microsoft-graph-preview"></a><span data-ttu-id="a4eba-103">Adicionar propriedades adicionais ao cartão de perfil usando a API de perfil no Microsoft Graph (visualização)</span><span class="sxs-lookup"><span data-stu-id="a4eba-103">Add additional properties to the profile card using the profile API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="a4eba-104">No [cartão de perfil](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) do Microsoft 365, você pode encontrar informações sobre os usuários que são armazenados e mantidos pela sua organização, por exemplo, **cargo** ou **local do escritório**.</span><span class="sxs-lookup"><span data-stu-id="a4eba-104">On the [profile card](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) in Microsoft 365, you can find information about users that is stored and maintained by your organization, for example **Job title** or **Office location**.</span></span>

<span data-ttu-id="a4eba-105">Use o recurso [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) para mostrar propriedades adicionais do Azure AD em cartões de perfil para uma organização, por:</span><span class="sxs-lookup"><span data-stu-id="a4eba-105">Use the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource to show additional properties from Azure AD on profile cards for an organization, by:</span></span>

- <span data-ttu-id="a4eba-106">Tornar mais atributos visíveis</span><span class="sxs-lookup"><span data-stu-id="a4eba-106">Making additional attributes visible</span></span>

- <span data-ttu-id="a4eba-107">Adicionando atributos personalizados</span><span class="sxs-lookup"><span data-stu-id="a4eba-107">Adding custom attributes</span></span>

<span data-ttu-id="a4eba-108">Propriedades adicionais serão exibidas na seção **contato** do cartão de perfil no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a4eba-108">Additional properties will display in the **Contact** section of the profile card in Microsoft 365.</span></span>

> [!NOTE]
><span data-ttu-id="a4eba-109">As operações no recurso **profileCardProperty** que usam permissões delegadas exigem que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="a4eba-109">Operations on the **profileCardProperty** resource that use delegated permissions requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="make-additional-attributes-visible"></a><span data-ttu-id="a4eba-110">Tornar mais atributos visíveis</span><span class="sxs-lookup"><span data-stu-id="a4eba-110">Make additional attributes visible</span></span>

<span data-ttu-id="a4eba-111">Você pode tornar os seguintes atributos do Azure Active Directory (Azure AD) visíveis nos cartões de perfil dos usuários.</span><span class="sxs-lookup"><span data-stu-id="a4eba-111">You can make the following attributes from Azure Active Directory (Azure AD) visible on users' profile cards.</span></span> <span data-ttu-id="a4eba-112">Esses atributos não diferenciam *maiúsculas de minúsculas*:</span><span class="sxs-lookup"><span data-stu-id="a4eba-112">These attributes are *not case-sensitive*:</span></span>

- `UserPrincipalName`
- `Fax`
- `StreetAddress`
- `PostalCode`
- `StateOrProvince`
- `Alias`

<span data-ttu-id="a4eba-113">A tabela a seguir mostra como os atributos do Azure AD correspondem às propriedades da entidade de [usuário](/graph/api/resources/user?view=graph-rest-beta) do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a4eba-113">The following table shows how the Azure AD attributes correspond with properties of the Microsoft Graph [user](/graph/api/resources/user?view=graph-rest-beta) entity.</span></span>

|<span data-ttu-id="a4eba-114">Atributo do Azure AD</span><span class="sxs-lookup"><span data-stu-id="a4eba-114">Azure AD attribute</span></span> |<span data-ttu-id="a4eba-115">Propriedade da entidade User</span><span class="sxs-lookup"><span data-stu-id="a4eba-115">User entity property</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a4eba-116">UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4eba-116">UserPrincipalName</span></span>|<span data-ttu-id="a4eba-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4eba-117">userPrincipalName</span></span> |
|<span data-ttu-id="a4eba-118">Fax</span><span class="sxs-lookup"><span data-stu-id="a4eba-118">Fax</span></span>|<span data-ttu-id="a4eba-119">faxNumber</span><span class="sxs-lookup"><span data-stu-id="a4eba-119">faxNumber</span></span>|
|<span data-ttu-id="a4eba-120">StreetAddress</span><span class="sxs-lookup"><span data-stu-id="a4eba-120">StreetAddress</span></span>|<span data-ttu-id="a4eba-121">streetAddress</span><span class="sxs-lookup"><span data-stu-id="a4eba-121">streetAddress</span></span>|
|<span data-ttu-id="a4eba-122">PostalCode</span><span class="sxs-lookup"><span data-stu-id="a4eba-122">PostalCode</span></span>|<span data-ttu-id="a4eba-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="a4eba-123">postalCode</span></span>|
|<span data-ttu-id="a4eba-124">StateOrProvince</span><span class="sxs-lookup"><span data-stu-id="a4eba-124">StateOrProvince</span></span>|<span data-ttu-id="a4eba-125">estado</span><span class="sxs-lookup"><span data-stu-id="a4eba-125">state</span></span>
|<span data-ttu-id="a4eba-126">Alias</span><span class="sxs-lookup"><span data-stu-id="a4eba-126">Alias</span></span>|<span data-ttu-id="a4eba-127">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a4eba-127">mailNickname</span></span>

<span data-ttu-id="a4eba-128">Você pode adicionar qualquer um desses atributos ao cartão de perfil definindo suas [configurações da organização](/graph/api/resources/organizationsettings?view=graph-rest-beta) e adicionando o atributo como a propriedade *directoryPropertyName*\* de um **profileCardProperty** no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a4eba-128">You can add any of these attributes to the profile card by configuring your [organization settings](/graph/api/resources/organizationsettings?view=graph-rest-beta) and adding the attribute as the *directoryPropertyName*\* property of a **profileCardProperty** in Microsoft Graph.</span></span> <span data-ttu-id="a4eba-129">Ao tornar mais atributos visíveis, você deve usar os nomes de propriedade para `en-us` .</span><span class="sxs-lookup"><span data-stu-id="a4eba-129">When you make additional attributes visible, you must use the property names for `en-us`.</span></span> <span data-ttu-id="a4eba-130">Você não precisa adicionar valores localizados.</span><span class="sxs-lookup"><span data-stu-id="a4eba-130">You don't have to add localized values.</span></span> <span data-ttu-id="a4eba-131">As propriedades adicionais serão exibidas automaticamente nas configurações de idioma que o usuário especificou para o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a4eba-131">The additional properties will automatically be shown in the language settings that the user has specified for Microsoft 365.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a4eba-132">Ao adicionar um atributo ao cartão de perfil, leva até 24 horas para que a adição seja exibida.</span><span class="sxs-lookup"><span data-stu-id="a4eba-132">When adding an attribute to profile card, it takes up to 24 hours for the addition to be displayed.</span></span>

## <a name="example"></a><span data-ttu-id="a4eba-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4eba-133">Example</span></span>

<span data-ttu-id="a4eba-134">O exemplo a seguir exibe o `Alias` atributo no cartão de perfil:</span><span class="sxs-lookup"><span data-stu-id="a4eba-134">The following example displays the `Alias` attribute on the profile card:</span></span>

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

<span data-ttu-id="a4eba-135">Se tiver êxito, a resposta retornará um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4eba-135">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="a4eba-136">O valor do `Alias` atributo seria exibido no cartão de perfil de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a4eba-136">The value for the `Alias` attribute  would be displayed on a user's profile card.</span></span>  

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a><span data-ttu-id="a4eba-137">Adicionando atributos personalizados</span><span class="sxs-lookup"><span data-stu-id="a4eba-137">Adding custom attributes</span></span>

<span data-ttu-id="a4eba-138">Você pode adicionar qualquer um dos 15 atributos de [extensão personalizada](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) do Azure ad aos cartões de perfil dos usuários, definindo suas configurações de organização e [adicionando o valor correspondente como um ProfileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a4eba-138">You can add any of the 15 Azure AD [custom extension attributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) to users' profile cards by configuring your organization settings and [adding the corresponding value as a profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) in Microsoft Graph.</span></span> <span data-ttu-id="a4eba-139">Você pode adicionar um recurso **profileCardProperty** por vez.</span><span class="sxs-lookup"><span data-stu-id="a4eba-139">You can add one **profileCardProperty** resource at a time.</span></span>

<span data-ttu-id="a4eba-140">É necessário até 24 horas para que as alterações sejam exibidas nos cartões de perfil.</span><span class="sxs-lookup"><span data-stu-id="a4eba-140">It takes up to 24 hours for the changes to show on profile cards.</span></span>

<span data-ttu-id="a4eba-141">As propriedades personalizadas não podem ser pesquisadas e não podem ser usadas para pesquisar pessoas em aplicativos e serviços da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a4eba-141">Custom properties are not searchable and can't be used to search for people across Microsoft apps and services.</span></span>

<span data-ttu-id="a4eba-142">A tabela a seguir mostra como os nomes de atributo de extensão personalizada do Azure AD correspondem aos valores com suporte para a propriedade **directoryPropertyName** do recurso [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="a4eba-142">The following table shows how the Azure AD custom extension attribute names correspond to the supported values for the **directoryPropertyName** property of the [profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta) resource.</span></span> <span data-ttu-id="a4eba-143">Esses nomes de atributos de extensão personalizada do Azure AD não diferenciam *maiúsculas de minúsculas*:</span><span class="sxs-lookup"><span data-stu-id="a4eba-143">These Azure AD custom extension attribute names are *not case-sensitive*:</span></span>

|<span data-ttu-id="a4eba-144">Atributo de extensão personalizada do Azure AD</span><span class="sxs-lookup"><span data-stu-id="a4eba-144">Azure AD custom extension attribute</span></span> | <span data-ttu-id="a4eba-145">Valor a ser especificado como directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="a4eba-145">Value to specify as directoryPropertyName</span></span> |
|:--------------------|:-----------------|
| <span data-ttu-id="a4eba-146">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="a4eba-146">extensionAttribute1</span></span> | <span data-ttu-id="a4eba-147">customAttribute1</span><span class="sxs-lookup"><span data-stu-id="a4eba-147">customAttribute1</span></span> |
| <span data-ttu-id="a4eba-148">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="a4eba-148">extensionAttribute2</span></span> | <span data-ttu-id="a4eba-149">customAttribute2</span><span class="sxs-lookup"><span data-stu-id="a4eba-149">customAttribute2</span></span> |
| <span data-ttu-id="a4eba-150">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="a4eba-150">extensionAttribute3</span></span> | <span data-ttu-id="a4eba-151">customAttribute3</span><span class="sxs-lookup"><span data-stu-id="a4eba-151">customAttribute3</span></span> |
| <span data-ttu-id="a4eba-152">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="a4eba-152">extensionAttribute4</span></span> | <span data-ttu-id="a4eba-153">customAttribute4</span><span class="sxs-lookup"><span data-stu-id="a4eba-153">customAttribute4</span></span> |
| <span data-ttu-id="a4eba-154">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="a4eba-154">extensionAttribute5</span></span> | <span data-ttu-id="a4eba-155">customAttribute5</span><span class="sxs-lookup"><span data-stu-id="a4eba-155">customAttribute5</span></span> |
| <span data-ttu-id="a4eba-156">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="a4eba-156">extensionAttribute6</span></span> | <span data-ttu-id="a4eba-157">customAttribute6</span><span class="sxs-lookup"><span data-stu-id="a4eba-157">customAttribute6</span></span> |
| <span data-ttu-id="a4eba-158">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="a4eba-158">extensionAttribute7</span></span> | <span data-ttu-id="a4eba-159">customAttribute7</span><span class="sxs-lookup"><span data-stu-id="a4eba-159">customAttribute7</span></span> |
| <span data-ttu-id="a4eba-160">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="a4eba-160">extensionAttribute8</span></span> | <span data-ttu-id="a4eba-161">customAttribute8</span><span class="sxs-lookup"><span data-stu-id="a4eba-161">customAttribute8</span></span> |
| <span data-ttu-id="a4eba-162">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="a4eba-162">extensionAttribute9</span></span> | <span data-ttu-id="a4eba-163">customAttribute9</span><span class="sxs-lookup"><span data-stu-id="a4eba-163">customAttribute9</span></span> |
| <span data-ttu-id="a4eba-164">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="a4eba-164">extensionAttribute10</span></span> | <span data-ttu-id="a4eba-165">customAttribute10</span><span class="sxs-lookup"><span data-stu-id="a4eba-165">customAttribute10</span></span> |
| <span data-ttu-id="a4eba-166">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="a4eba-166">extensionAttribute11</span></span> | <span data-ttu-id="a4eba-167">customAttribute11</span><span class="sxs-lookup"><span data-stu-id="a4eba-167">customAttribute11</span></span> |
| <span data-ttu-id="a4eba-168">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="a4eba-168">extensionAttribute12</span></span> | <span data-ttu-id="a4eba-169">customAttribute12</span><span class="sxs-lookup"><span data-stu-id="a4eba-169">customAttribute12</span></span> |
| <span data-ttu-id="a4eba-170">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="a4eba-170">extensionAttribute13</span></span> | <span data-ttu-id="a4eba-171">customAttribute13</span><span class="sxs-lookup"><span data-stu-id="a4eba-171">customAttribute13</span></span> |
| <span data-ttu-id="a4eba-172">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="a4eba-172">extensionAttribute14</span></span> | <span data-ttu-id="a4eba-173">customAttribute14</span><span class="sxs-lookup"><span data-stu-id="a4eba-173">customAttribute14</span></span> |
| <span data-ttu-id="a4eba-174">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="a4eba-174">extensionAttribute15</span></span> | <span data-ttu-id="a4eba-175">customAttribute15</span><span class="sxs-lookup"><span data-stu-id="a4eba-175">customAttribute15</span></span> |

## <a name="example"></a><span data-ttu-id="a4eba-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4eba-176">Example</span></span>

<span data-ttu-id="a4eba-177">O exemplo a seguir adiciona o primeiro atributo de extensão personalizado do Azure AD ao cartão de perfil, usando o nome de exibição **central de custos**.</span><span class="sxs-lookup"><span data-stu-id="a4eba-177">The following example adds the first Azure AD custom extension attribute to the profile card, using the display name **Cost center**.</span></span> <span data-ttu-id="a4eba-178">Para usuários que definiram suas configurações de idioma como alemão, o nome de exibição será **Kostenstelle**.</span><span class="sxs-lookup"><span data-stu-id="a4eba-178">For users that have set their language settings to German, the display name will be **Kostenstelle**.</span></span>

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

<span data-ttu-id="a4eba-179">Se não houver suporte para um idioma, o nome da propriedade será mostrado com o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="a4eba-179">If a language is not supported, the property name will be shown with the default value.</span></span>  

<span data-ttu-id="a4eba-180">Se tiver êxito, a resposta retornará um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4eba-180">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="a4eba-181">Neste exemplo, você pode supor que o cartão de perfil exibe **Kostenstelle** para todos os usuários que definiram suas configurações de idioma como alemão no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="a4eba-181">In this example you can assume that the profile card displays **Kostenstelle** for all users that have set their language settings to German on the profile card.</span></span> <span data-ttu-id="a4eba-182">Para todos os outros usuários, o **centro de custos** será exibido no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="a4eba-182">For all other users, **Cost center** will be displayed on the profile card.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a4eba-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="a4eba-183">See also</span></span>

[<span data-ttu-id="a4eba-184">Encontre sua ID de locatário do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a4eba-184">Find your Microsoft 365 tenant ID</span></span>](https://docs.microsoft.com/onedrive/find-your-office-365-tenant-id)

[<span data-ttu-id="a4eba-185">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="a4eba-185">onPremisesExtensionAttributes resource type</span></span>](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)

[<span data-ttu-id="a4eba-186">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="a4eba-186">User resource type</span></span>](/graph/api/resources/user?view=graph-rest-beta)

[<span data-ttu-id="a4eba-187">Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="a4eba-187">Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer)

[<span data-ttu-id="a4eba-188">Obter profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="a4eba-188">Get profileCardProperty</span></span>](/graph/api/profilecardproperty-get?view=graph-rest-beta)
