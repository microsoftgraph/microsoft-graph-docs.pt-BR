---
title: Atualizar microsoftStoreForBusinessApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e23afba48af0ad72c90d288684cc7cecadb8c65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140940"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="26876-103">Atualizar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="26876-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="26876-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26876-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26876-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26876-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26876-106">Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="26876-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26876-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26876-107">Prerequisites</span></span>
<span data-ttu-id="26876-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="26876-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="26876-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26876-110">Permission type</span></span>|<span data-ttu-id="26876-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26876-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26876-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26876-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26876-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26876-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26876-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26876-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26876-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26876-115">Not supported.</span></span>|
|<span data-ttu-id="26876-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26876-116">Application</span></span>|<span data-ttu-id="26876-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26876-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26876-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26876-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="26876-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26876-119">Request headers</span></span>
|<span data-ttu-id="26876-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26876-120">Header</span></span>|<span data-ttu-id="26876-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26876-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26876-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26876-122">Authorization</span></span>|<span data-ttu-id="26876-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26876-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26876-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26876-124">Accept</span></span>|<span data-ttu-id="26876-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26876-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26876-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26876-126">Request body</span></span>
<span data-ttu-id="26876-127">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="26876-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="26876-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="26876-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="26876-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26876-129">Property</span></span>|<span data-ttu-id="26876-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="26876-130">Type</span></span>|<span data-ttu-id="26876-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="26876-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26876-132">id</span><span class="sxs-lookup"><span data-stu-id="26876-132">id</span></span>|<span data-ttu-id="26876-133">String</span><span class="sxs-lookup"><span data-stu-id="26876-133">String</span></span>|<span data-ttu-id="26876-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26876-134">Key of the entity.</span></span> <span data-ttu-id="26876-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-136">displayName</span><span class="sxs-lookup"><span data-stu-id="26876-136">displayName</span></span>|<span data-ttu-id="26876-137">String</span><span class="sxs-lookup"><span data-stu-id="26876-137">String</span></span>|<span data-ttu-id="26876-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="26876-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="26876-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-140">description</span><span class="sxs-lookup"><span data-stu-id="26876-140">description</span></span>|<span data-ttu-id="26876-141">String</span><span class="sxs-lookup"><span data-stu-id="26876-141">String</span></span>|<span data-ttu-id="26876-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26876-142">The description of the app.</span></span> <span data-ttu-id="26876-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-144">publisher</span><span class="sxs-lookup"><span data-stu-id="26876-144">publisher</span></span>|<span data-ttu-id="26876-145">String</span><span class="sxs-lookup"><span data-stu-id="26876-145">String</span></span>|<span data-ttu-id="26876-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26876-146">The publisher of the app.</span></span> <span data-ttu-id="26876-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="26876-148">largeIcon</span></span>|[<span data-ttu-id="26876-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="26876-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="26876-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="26876-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="26876-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26876-152">createdDateTime</span></span>|<span data-ttu-id="26876-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26876-153">DateTimeOffset</span></span>|<span data-ttu-id="26876-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26876-154">The date and time the app was created.</span></span> <span data-ttu-id="26876-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26876-156">lastModifiedDateTime</span></span>|<span data-ttu-id="26876-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26876-157">DateTimeOffset</span></span>|<span data-ttu-id="26876-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="26876-158">The date and time the app was last modified.</span></span> <span data-ttu-id="26876-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="26876-160">isFeatured</span></span>|<span data-ttu-id="26876-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="26876-161">Boolean</span></span>|<span data-ttu-id="26876-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="26876-163">privacyInformationUrl</span></span>|<span data-ttu-id="26876-164">String</span><span class="sxs-lookup"><span data-stu-id="26876-164">String</span></span>|<span data-ttu-id="26876-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="26876-165">The privacy statement Url.</span></span> <span data-ttu-id="26876-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="26876-167">informationUrl</span></span>|<span data-ttu-id="26876-168">String</span><span class="sxs-lookup"><span data-stu-id="26876-168">String</span></span>|<span data-ttu-id="26876-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="26876-169">The more information Url.</span></span> <span data-ttu-id="26876-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-171">owner</span><span class="sxs-lookup"><span data-stu-id="26876-171">owner</span></span>|<span data-ttu-id="26876-172">String</span><span class="sxs-lookup"><span data-stu-id="26876-172">String</span></span>|<span data-ttu-id="26876-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="26876-173">The owner of the app.</span></span> <span data-ttu-id="26876-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-175">developer</span><span class="sxs-lookup"><span data-stu-id="26876-175">developer</span></span>|<span data-ttu-id="26876-176">String</span><span class="sxs-lookup"><span data-stu-id="26876-176">String</span></span>|<span data-ttu-id="26876-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26876-177">The developer of the app.</span></span> <span data-ttu-id="26876-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-179">Observações</span><span class="sxs-lookup"><span data-stu-id="26876-179">notes</span></span>|<span data-ttu-id="26876-180">String</span><span class="sxs-lookup"><span data-stu-id="26876-180">String</span></span>|<span data-ttu-id="26876-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26876-181">Notes for the app.</span></span> <span data-ttu-id="26876-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="26876-183">uploadState</span></span>|<span data-ttu-id="26876-184">Int32</span><span class="sxs-lookup"><span data-stu-id="26876-184">Int32</span></span>|<span data-ttu-id="26876-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="26876-185">The upload state.</span></span> <span data-ttu-id="26876-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="26876-187">publishingState</span></span>|[<span data-ttu-id="26876-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="26876-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="26876-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26876-189">The publishing state for the app.</span></span> <span data-ttu-id="26876-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="26876-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="26876-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="26876-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="26876-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="26876-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="26876-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="26876-193">isAssigned</span></span>|<span data-ttu-id="26876-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="26876-194">Boolean</span></span>|<span data-ttu-id="26876-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="26876-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="26876-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26876-197">roleScopeTagIds</span></span>|<span data-ttu-id="26876-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="26876-198">String collection</span></span>|<span data-ttu-id="26876-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="26876-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="26876-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="26876-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="26876-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="26876-201">usedLicenseCount</span></span>|<span data-ttu-id="26876-202">Int32</span><span class="sxs-lookup"><span data-stu-id="26876-202">Int32</span></span>|<span data-ttu-id="26876-203">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="26876-203">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="26876-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="26876-204">totalLicenseCount</span></span>|<span data-ttu-id="26876-205">Int32</span><span class="sxs-lookup"><span data-stu-id="26876-205">Int32</span></span>|<span data-ttu-id="26876-206">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="26876-206">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="26876-207">productKey</span><span class="sxs-lookup"><span data-stu-id="26876-207">productKey</span></span>|<span data-ttu-id="26876-208">String</span><span class="sxs-lookup"><span data-stu-id="26876-208">String</span></span>|<span data-ttu-id="26876-209">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="26876-209">The app product key</span></span>|
|<span data-ttu-id="26876-210">licenseType</span><span class="sxs-lookup"><span data-stu-id="26876-210">licenseType</span></span>|[<span data-ttu-id="26876-211">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="26876-211">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="26876-212">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26876-212">The app license type.</span></span> <span data-ttu-id="26876-213">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="26876-213">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="26876-214">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="26876-214">packageIdentityName</span></span>|<span data-ttu-id="26876-215">String</span><span class="sxs-lookup"><span data-stu-id="26876-215">String</span></span>|<span data-ttu-id="26876-216">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="26876-216">The app package identifier</span></span>|
|<span data-ttu-id="26876-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="26876-217">licensingType</span></span>|[<span data-ttu-id="26876-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="26876-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="26876-219">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="26876-219">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="26876-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="26876-220">Response</span></span>
<span data-ttu-id="26876-221">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26876-221">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26876-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26876-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="26876-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26876-223">Request</span></span>
<span data-ttu-id="26876-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26876-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1105

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
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="26876-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="26876-225">Response</span></span>
<span data-ttu-id="26876-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26876-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

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
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```




