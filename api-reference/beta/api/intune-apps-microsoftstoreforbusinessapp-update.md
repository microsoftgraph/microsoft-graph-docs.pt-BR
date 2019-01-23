---
title: Atualizar microsoftStoreForBusinessApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5f2bee3e2cbbdd1f02bbd7a1779ea80b2340772
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417494"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="4bb65-103">Atualizar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="4bb65-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="4bb65-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bb65-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4bb65-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bb65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4bb65-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4bb65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bb65-107">Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4bb65-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bb65-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4bb65-108">Prerequisites</span></span>
<span data-ttu-id="4bb65-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bb65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4bb65-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bb65-111">Permission type</span></span>|<span data-ttu-id="4bb65-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4bb65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bb65-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bb65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bb65-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bb65-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4bb65-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bb65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bb65-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bb65-116">Not supported.</span></span>|
|<span data-ttu-id="4bb65-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bb65-117">Application</span></span>|<span data-ttu-id="4bb65-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bb65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bb65-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bb65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4bb65-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bb65-120">Request headers</span></span>
|<span data-ttu-id="4bb65-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bb65-121">Header</span></span>|<span data-ttu-id="4bb65-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4bb65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bb65-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bb65-123">Authorization</span></span>|<span data-ttu-id="4bb65-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bb65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bb65-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4bb65-125">Accept</span></span>|<span data-ttu-id="4bb65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bb65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bb65-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bb65-127">Request body</span></span>
<span data-ttu-id="4bb65-128">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4bb65-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="4bb65-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4bb65-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="4bb65-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bb65-130">Property</span></span>|<span data-ttu-id="4bb65-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bb65-131">Type</span></span>|<span data-ttu-id="4bb65-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bb65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb65-133">id</span><span class="sxs-lookup"><span data-stu-id="4bb65-133">id</span></span>|<span data-ttu-id="4bb65-134">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-134">String</span></span>|<span data-ttu-id="4bb65-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4bb65-135">Key of the entity.</span></span> <span data-ttu-id="4bb65-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4bb65-137">displayName</span></span>|<span data-ttu-id="4bb65-138">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-138">String</span></span>|<span data-ttu-id="4bb65-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4bb65-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4bb65-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-141">description</span><span class="sxs-lookup"><span data-stu-id="4bb65-141">description</span></span>|<span data-ttu-id="4bb65-142">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-142">String</span></span>|<span data-ttu-id="4bb65-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-143">The description of the app.</span></span> <span data-ttu-id="4bb65-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4bb65-145">publisher</span></span>|<span data-ttu-id="4bb65-146">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-146">String</span></span>|<span data-ttu-id="4bb65-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-147">The publisher of the app.</span></span> <span data-ttu-id="4bb65-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4bb65-149">largeIcon</span></span>|[<span data-ttu-id="4bb65-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4bb65-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4bb65-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4bb65-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4bb65-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bb65-153">createdDateTime</span></span>|<span data-ttu-id="4bb65-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bb65-154">DateTimeOffset</span></span>|<span data-ttu-id="4bb65-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-155">The date and time the app was created.</span></span> <span data-ttu-id="4bb65-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bb65-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4bb65-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bb65-158">DateTimeOffset</span></span>|<span data-ttu-id="4bb65-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4bb65-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4bb65-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4bb65-161">isFeatured</span></span>|<span data-ttu-id="4bb65-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bb65-162">Boolean</span></span>|<span data-ttu-id="4bb65-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4bb65-164">privacyInformationUrl</span></span>|<span data-ttu-id="4bb65-165">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-165">String</span></span>|<span data-ttu-id="4bb65-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4bb65-166">The privacy statement Url.</span></span> <span data-ttu-id="4bb65-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4bb65-168">informationUrl</span></span>|<span data-ttu-id="4bb65-169">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-169">String</span></span>|<span data-ttu-id="4bb65-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4bb65-170">The more information Url.</span></span> <span data-ttu-id="4bb65-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-172">owner</span><span class="sxs-lookup"><span data-stu-id="4bb65-172">owner</span></span>|<span data-ttu-id="4bb65-173">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-173">String</span></span>|<span data-ttu-id="4bb65-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-174">The owner of the app.</span></span> <span data-ttu-id="4bb65-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-176">developer</span><span class="sxs-lookup"><span data-stu-id="4bb65-176">developer</span></span>|<span data-ttu-id="4bb65-177">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-177">String</span></span>|<span data-ttu-id="4bb65-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-178">The developer of the app.</span></span> <span data-ttu-id="4bb65-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-180">Observações</span><span class="sxs-lookup"><span data-stu-id="4bb65-180">notes</span></span>|<span data-ttu-id="4bb65-181">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-181">String</span></span>|<span data-ttu-id="4bb65-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-182">Notes for the app.</span></span> <span data-ttu-id="4bb65-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4bb65-184">uploadState</span></span>|<span data-ttu-id="4bb65-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4bb65-185">Int32</span></span>|<span data-ttu-id="4bb65-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="4bb65-186">The upload state.</span></span> <span data-ttu-id="4bb65-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4bb65-188">publishingState</span></span>|[<span data-ttu-id="4bb65-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4bb65-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4bb65-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-190">The publishing state for the app.</span></span> <span data-ttu-id="4bb65-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4bb65-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4bb65-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4bb65-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4bb65-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4bb65-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4bb65-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4bb65-194">isAssigned</span></span>|<span data-ttu-id="4bb65-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bb65-195">Boolean</span></span>|<span data-ttu-id="4bb65-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4bb65-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4bb65-198">roleScopeTagIds</span></span>|<span data-ttu-id="4bb65-199">String collection</span><span class="sxs-lookup"><span data-stu-id="4bb65-199">String collection</span></span>|<span data-ttu-id="4bb65-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4bb65-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4bb65-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bb65-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4bb65-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4bb65-202">usedLicenseCount</span></span>|<span data-ttu-id="4bb65-203">Int32</span><span class="sxs-lookup"><span data-stu-id="4bb65-203">Int32</span></span>|<span data-ttu-id="4bb65-204">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="4bb65-204">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="4bb65-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4bb65-205">totalLicenseCount</span></span>|<span data-ttu-id="4bb65-206">Int32</span><span class="sxs-lookup"><span data-stu-id="4bb65-206">Int32</span></span>|<span data-ttu-id="4bb65-207">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="4bb65-207">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="4bb65-208">productKey</span><span class="sxs-lookup"><span data-stu-id="4bb65-208">productKey</span></span>|<span data-ttu-id="4bb65-209">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-209">String</span></span>|<span data-ttu-id="4bb65-210">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bb65-210">The app product key</span></span>|
|<span data-ttu-id="4bb65-211">licenseType</span><span class="sxs-lookup"><span data-stu-id="4bb65-211">licenseType</span></span>|[<span data-ttu-id="4bb65-212">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="4bb65-212">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="4bb65-213">O tipo de licença de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4bb65-213">The app license type.</span></span> <span data-ttu-id="4bb65-214">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="4bb65-214">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="4bb65-215">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="4bb65-215">packageIdentityName</span></span>|<span data-ttu-id="4bb65-216">String</span><span class="sxs-lookup"><span data-stu-id="4bb65-216">String</span></span>|<span data-ttu-id="4bb65-217">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bb65-217">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="4bb65-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bb65-218">Response</span></span>
<span data-ttu-id="4bb65-219">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bb65-219">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bb65-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bb65-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bb65-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bb65-221">Request</span></span>
<span data-ttu-id="4bb65-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bb65-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 876

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="4bb65-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bb65-223">Response</span></span>
<span data-ttu-id="4bb65-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bb65-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```




