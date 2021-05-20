---
title: Personalizar o cartão de perfil usando a API de perfil no Microsoft Graph (visualização)
description: Este artigo descreve como você pode personalizar o cartão de perfil tornando visíveis atributos adicionais ou adicionando atributos personalizados.
author: PollyNincevic
localization\_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 527afbad1ef35e4fba9fe0360accb19ae3ae9ead
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547159"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-card-api-in-microsoft-graph-preview"></a><span data-ttu-id="ae1f5-103">Adicionar propriedades adicionais ao cartão de perfil usando a API do cartão de perfil no Microsoft Graph (visualização)</span><span class="sxs-lookup"><span data-stu-id="ae1f5-103">Add additional properties to the profile card using the profile card API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="ae1f5-104">No [cartão de perfil](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) no Microsoft 365, você pode encontrar informações sobre os usuários armazenados e mantidos pela sua organização, por exemplo **Título do cargo** ou **Local do escritório**.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-104">On the [profile card](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) in Microsoft 365, you can find information about users that is stored and maintained by your organization, for example **Job title** or **Office location**.</span></span>

<span data-ttu-id="ae1f5-105">Use o recurso [profileCardProperty](/graph/api/resources/profilecardproperty) para mostrar propriedades adicionais do Microsoft Azure Active Directory em cartões de perfil de uma organização:</span><span class="sxs-lookup"><span data-stu-id="ae1f5-105">Use the [profileCardProperty](/graph/api/resources/profilecardproperty) resource to show additional properties from Azure AD on profile cards for an organization, by:</span></span>

* <span data-ttu-id="ae1f5-106">Tornando visíveis atributos adicionais</span><span class="sxs-lookup"><span data-stu-id="ae1f5-106">Making additional attributes visible</span></span>
* <span data-ttu-id="ae1f5-107">Adicionando atributos personalizados</span><span class="sxs-lookup"><span data-stu-id="ae1f5-107">Adding custom attributes</span></span>

<span data-ttu-id="ae1f5-108">As propriedades adicionais serão exibidas na seção **Contato** do cartão de perfil no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-108">Additional properties will display in the **Contact** section of the profile card in Microsoft 365.</span></span>

> [!NOTE]
> <span data-ttu-id="ae1f5-109">As operações no **recurso profileCardProperty** que usam permissões delegadas exigem que o usuário de entrada tenha um administrador de locatário ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-109">Operations on the **profileCardProperty** resource that use delegated permissions require the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="make-additional-attributes-visible"></a><span data-ttu-id="ae1f5-110">Torne visíveis atributos adicionais</span><span class="sxs-lookup"><span data-stu-id="ae1f5-110">Make additional attributes visible</span></span>

<span data-ttu-id="ae1f5-111">Você pode fazer os seguintes atributos do Azure Active Directory (Azure AD) visíveis nos cartões de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-111">You can make the following attributes from Azure Active Directory (Azure AD) visible on users' profile cards.</span></span> <span data-ttu-id="ae1f5-112">Esses atributos *não diferenciam maiúsculas de minúsculas*:</span><span class="sxs-lookup"><span data-stu-id="ae1f5-112">These attributes are *not case-sensitive*:</span></span>

* `UserPrincipalName`
* `Fax`
* `StreetAddress`
* `PostalCode`
* `StateOrProvince`
* `Alias`

<span data-ttu-id="ae1f5-113">A tabela a seguir mostra como os atributos do Azure AD correspondem com as propriedades da entidade [user](/graph/api/resources/user) do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-113">The following table shows how the Azure AD attributes correspond with properties of the Microsoft Graph [user](/graph/api/resources/user) entity.</span></span>

| <span data-ttu-id="ae1f5-114">Atributo do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="ae1f5-114">Azure AD attribute</span></span> | <span data-ttu-id="ae1f5-115">Propriedade da entidade User</span><span class="sxs-lookup"><span data-stu-id="ae1f5-115">User entity property</span></span> |
| ------------------ | -------------------- |
| <span data-ttu-id="ae1f5-116">UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae1f5-116">UserPrincipalName</span></span> | <span data-ttu-id="ae1f5-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae1f5-117">userPrincipalName</span></span> |
| <span data-ttu-id="ae1f5-118">Fax</span><span class="sxs-lookup"><span data-stu-id="ae1f5-118">Fax</span></span> | <span data-ttu-id="ae1f5-119">faxNumber</span><span class="sxs-lookup"><span data-stu-id="ae1f5-119">faxNumber</span></span> |
| <span data-ttu-id="ae1f5-120">StreetAddress</span><span class="sxs-lookup"><span data-stu-id="ae1f5-120">StreetAddress</span></span> | <span data-ttu-id="ae1f5-121">streetAddress</span><span class="sxs-lookup"><span data-stu-id="ae1f5-121">streetAddress</span></span> |
| <span data-ttu-id="ae1f5-122">PostalCode</span><span class="sxs-lookup"><span data-stu-id="ae1f5-122">PostalCode</span></span> | <span data-ttu-id="ae1f5-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="ae1f5-123">postalCode</span></span> |
| <span data-ttu-id="ae1f5-124">StateOrProvince</span><span class="sxs-lookup"><span data-stu-id="ae1f5-124">StateOrProvince</span></span> | <span data-ttu-id="ae1f5-125">estado</span><span class="sxs-lookup"><span data-stu-id="ae1f5-125">state</span></span> |
| <span data-ttu-id="ae1f5-126">Alias</span><span class="sxs-lookup"><span data-stu-id="ae1f5-126">Alias</span></span> | <span data-ttu-id="ae1f5-127">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ae1f5-127">mailNickname</span></span> |

<span data-ttu-id="ae1f5-128">Você pode adicionar qualquer um desses atributos ao [](/graph/api/resources/organizationsettings) cartão de perfil configurando as configurações da sua organização e adicionando o atributo como a **propriedade directoryPropertyName** de **um profileCardProperty** no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-128">You can add any of these attributes to the profile card by configuring your [organization settings](/graph/api/resources/organizationsettings) and adding the attribute as the **directoryPropertyName** property of a **profileCardProperty** in Microsoft Graph.</span></span> <span data-ttu-id="ae1f5-129">Ao tornar visíveis atributos adicionais, você deve usar os nomes de propriedades para `en-us`.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-129">When you make additional attributes visible, you must use the property names for `en-us`.</span></span> <span data-ttu-id="ae1f5-130">Não é necessário adicionar valores localizados.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-130">You don't have to add localized values.</span></span> <span data-ttu-id="ae1f5-131">As propriedades adicionais serão exibidas automaticamente nas configurações de idioma especificadas para o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-131">The additional properties will automatically be shown in the language settings that the user has specified for Microsoft 365.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ae1f5-132">Ao adicionar um atributo ao cartão de perfil, leva até 24 horas para que a adição seja exibida.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-132">When adding an attribute to profile card, it takes up to 24 hours for the addition to be displayed.</span></span>

### <a name="example"></a><span data-ttu-id="ae1f5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae1f5-133">Example</span></span>

<span data-ttu-id="ae1f5-134">O exemplo a seguir exibe o `Alias` atributo no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-134">The following example displays the `Alias` attribute on the profile card.</span></span>

``` http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

<span data-ttu-id="ae1f5-135">Se bem-sucedido, este método retorna um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-135">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="ae1f5-136">O valor do `Alias` atributo seria exibido no cartão de perfil de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-136">The value for the `Alias` attribute would be displayed on a user's profile card.</span></span>

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a><span data-ttu-id="ae1f5-137">Adicionando atributos personalizados</span><span class="sxs-lookup"><span data-stu-id="ae1f5-137">Adding custom attributes</span></span>

<span data-ttu-id="ae1f5-138">Você pode adicionar qualquer um dos 15 [atributos de extensão personalizada](/graph/api/resources/onpremisesextensionattributes) do Azure AD aos cartões de perfil do usuário, definindo as configurações da sua organização e [adicionando o valor correspondente como um profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-138">You can add any of the 15 Azure AD [custom extension attributes](/graph/api/resources/onpremisesextensionattributes) to users' profile cards by configuring your organization settings and [adding the corresponding value as a profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties) in Microsoft Graph.</span></span> <span data-ttu-id="ae1f5-139">Você pode adicionar um recurso **profileCardProperty** por vez.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-139">You can add one **profileCardProperty** resource at a time.</span></span>

<span data-ttu-id="ae1f5-140">São necessárias até 24 horas para que as alterações sejam mostradas em cartões de perfil.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-140">It takes up to 24 hours for the changes to show on profile cards.</span></span>

<span data-ttu-id="ae1f5-141">As propriedades personalizadas não podem ser pesquisadas e não podem ser usadas para pesquisar pessoas em serviços e aplicativos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-141">Custom properties are not searchable and can't be used to search for people across Microsoft apps and services.</span></span>

<span data-ttu-id="ae1f5-142">A tabela a seguir mostra como os nomes de atributos de extensão personalizada do Microsoft Azure Active Directory correspondem aos valores com suporte para a propriedade **directoryPropertyName** do recurso [profileCardProperty](/graph/api/resources/profilecardproperty).</span><span class="sxs-lookup"><span data-stu-id="ae1f5-142">The following table shows how the Azure AD custom extension attribute names correspond to the supported values for the **directoryPropertyName** property of the [profileCardProperty](/graph/api/resources/profilecardproperty) resource.</span></span> <span data-ttu-id="ae1f5-143">Esses nomes de atributos de extensão personalizada do Microsoft Azure Active Directory *não fazem distinção entre maiúsculas e minúsculas*:</span><span class="sxs-lookup"><span data-stu-id="ae1f5-143">These Azure AD custom extension attribute names are *not case-sensitive*:</span></span>

| <span data-ttu-id="ae1f5-144">Atributo de extensão personalizada do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="ae1f5-144">Azure AD custom extension attribute</span></span> | <span data-ttu-id="ae1f5-145">Valor para especificar como directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="ae1f5-145">Value to specify as directoryPropertyName</span></span> |
| ----------------------------------- | ----------------------------------------- |
| <span data-ttu-id="ae1f5-146">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="ae1f5-146">extensionAttribute1</span></span> | <span data-ttu-id="ae1f5-147">customAttribute1</span><span class="sxs-lookup"><span data-stu-id="ae1f5-147">customAttribute1</span></span> |
| <span data-ttu-id="ae1f5-148">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="ae1f5-148">extensionAttribute2</span></span> | <span data-ttu-id="ae1f5-149">customAttribute2</span><span class="sxs-lookup"><span data-stu-id="ae1f5-149">customAttribute2</span></span> |
| <span data-ttu-id="ae1f5-150">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="ae1f5-150">extensionAttribute3</span></span> | <span data-ttu-id="ae1f5-151">customAttribute3</span><span class="sxs-lookup"><span data-stu-id="ae1f5-151">customAttribute3</span></span> |
| <span data-ttu-id="ae1f5-152">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="ae1f5-152">extensionAttribute4</span></span> | <span data-ttu-id="ae1f5-153">customAttribute4</span><span class="sxs-lookup"><span data-stu-id="ae1f5-153">customAttribute4</span></span> |
| <span data-ttu-id="ae1f5-154">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="ae1f5-154">extensionAttribute5</span></span> | <span data-ttu-id="ae1f5-155">customAttribute5</span><span class="sxs-lookup"><span data-stu-id="ae1f5-155">customAttribute5</span></span> |
| <span data-ttu-id="ae1f5-156">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="ae1f5-156">extensionAttribute6</span></span> | <span data-ttu-id="ae1f5-157">customAttribute6</span><span class="sxs-lookup"><span data-stu-id="ae1f5-157">customAttribute6</span></span> |
| <span data-ttu-id="ae1f5-158">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="ae1f5-158">extensionAttribute7</span></span> | <span data-ttu-id="ae1f5-159">customAttribute7</span><span class="sxs-lookup"><span data-stu-id="ae1f5-159">customAttribute7</span></span> |
| <span data-ttu-id="ae1f5-160">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="ae1f5-160">extensionAttribute8</span></span> | <span data-ttu-id="ae1f5-161">customAttribute8</span><span class="sxs-lookup"><span data-stu-id="ae1f5-161">customAttribute8</span></span> |
| <span data-ttu-id="ae1f5-162">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="ae1f5-162">extensionAttribute9</span></span> | <span data-ttu-id="ae1f5-163">customAttribute9</span><span class="sxs-lookup"><span data-stu-id="ae1f5-163">customAttribute9</span></span> |
| <span data-ttu-id="ae1f5-164">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="ae1f5-164">extensionAttribute10</span></span> | <span data-ttu-id="ae1f5-165">customAttribute10</span><span class="sxs-lookup"><span data-stu-id="ae1f5-165">customAttribute10</span></span> |
| <span data-ttu-id="ae1f5-166">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="ae1f5-166">extensionAttribute11</span></span> | <span data-ttu-id="ae1f5-167">customAttribute11</span><span class="sxs-lookup"><span data-stu-id="ae1f5-167">customAttribute11</span></span> |
| <span data-ttu-id="ae1f5-168">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="ae1f5-168">extensionAttribute12</span></span> | <span data-ttu-id="ae1f5-169">customAttribute12</span><span class="sxs-lookup"><span data-stu-id="ae1f5-169">customAttribute12</span></span> |
| <span data-ttu-id="ae1f5-170">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="ae1f5-170">extensionAttribute13</span></span> | <span data-ttu-id="ae1f5-171">customAttribute13</span><span class="sxs-lookup"><span data-stu-id="ae1f5-171">customAttribute13</span></span> |
| <span data-ttu-id="ae1f5-172">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="ae1f5-172">extensionAttribute14</span></span> | <span data-ttu-id="ae1f5-173">customAttribute14</span><span class="sxs-lookup"><span data-stu-id="ae1f5-173">customAttribute14</span></span> |
| <span data-ttu-id="ae1f5-174">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="ae1f5-174">extensionAttribute15</span></span> | <span data-ttu-id="ae1f5-175">customAttribute15</span><span class="sxs-lookup"><span data-stu-id="ae1f5-175">customAttribute15</span></span> |

### <a name="example"></a><span data-ttu-id="ae1f5-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae1f5-176">Example</span></span>

<span data-ttu-id="ae1f5-177">O exemplo a seguir adiciona o primeiro atributo de extensão personalizada do Microsoft Azure Active Directory para o cartão de perfil, usando o nome de exibição **Centro de custos**.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-177">The following example adds the first Azure AD custom extension attribute to the profile card, using the display name **Cost center**.</span></span> <span data-ttu-id="ae1f5-178">Para os usuários que definiram as configurações de idioma para o alemão, o nome de exibição será **Kostenstelle**.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-178">For users that have set their language settings to German, the display name will be **Kostenstelle**.</span></span>

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

<span data-ttu-id="ae1f5-179">Se não houver suporte a um idioma, o nome da propriedade será mostrado com o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-179">If a language is not supported, the property name will be shown with the default value.</span></span>

<span data-ttu-id="ae1f5-180">Se bem-sucedido, este método retorna um `201 OK` código de resposta e um objeto **profileCardProperty** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-180">If successful, the response returns a `201 OK` response code and a **profileCardProperty** object in the response body.</span></span> <span data-ttu-id="ae1f5-181">Neste exemplo, você pode supor que o cartão de perfil exiba **Kostenstelle** para todos os usuários que definiram as configurações de idioma para o alemão no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-181">In this example you can assume that the profile card displays **Kostenstelle** for all users that have set their language settings to German on the profile card.</span></span> <span data-ttu-id="ae1f5-182">Para todos os outros usuários, **Centro de custos** será exibido no cartão de perfil.</span><span class="sxs-lookup"><span data-stu-id="ae1f5-182">For all other users, **Cost center** will be displayed on the profile card.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ae1f5-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="ae1f5-183">See also</span></span>

- [<span data-ttu-id="ae1f5-184">Localizar sua ID de locatário do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ae1f5-184">Find your Microsoft 365 tenant ID</span></span>](/onedrive/find-your-office-365-tenant-id)
- [<span data-ttu-id="ae1f5-185">Tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="ae1f5-185">onPremisesExtensionAttributes resource type</span></span>](/graph/api/resources/onpremisesextensionattributes)
- [<span data-ttu-id="ae1f5-186">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="ae1f5-186">User resource type</span></span>](/graph/api/resources/user)
- [<span data-ttu-id="ae1f5-187">Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="ae1f5-187">Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer)
- [<span data-ttu-id="ae1f5-188">Obter profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="ae1f5-188">Get profileCardProperty</span></span>](/graph/api/profilecardproperty-get)
