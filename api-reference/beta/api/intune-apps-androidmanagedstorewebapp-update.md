---
title: Atualizar androidManagedStoreWebApp
description: Atualiza as propriedades de um objeto androidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3b61e97083819d3f5a5082d02a1bd5902431e44
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417311"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="1dae7-103">Atualizar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="1dae7-103">Update androidManagedStoreWebApp</span></span>

<span data-ttu-id="1dae7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dae7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dae7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1dae7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dae7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1dae7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dae7-107">Atualiza as propriedades de um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="1dae7-107">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dae7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1dae7-108">Prerequisites</span></span>
<span data-ttu-id="1dae7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dae7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dae7-111">Permission type</span></span>|<span data-ttu-id="1dae7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1dae7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dae7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dae7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1dae7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dae7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1dae7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dae7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dae7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dae7-116">Not supported.</span></span>|
|<span data-ttu-id="1dae7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dae7-117">Application</span></span>|<span data-ttu-id="1dae7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dae7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dae7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dae7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1dae7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dae7-120">Request headers</span></span>
|<span data-ttu-id="1dae7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1dae7-121">Header</span></span>|<span data-ttu-id="1dae7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1dae7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dae7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dae7-123">Authorization</span></span>|<span data-ttu-id="1dae7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dae7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dae7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1dae7-125">Accept</span></span>|<span data-ttu-id="1dae7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1dae7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dae7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dae7-127">Request body</span></span>
<span data-ttu-id="1dae7-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="1dae7-128">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="1dae7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span><span class="sxs-lookup"><span data-stu-id="1dae7-129">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="1dae7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dae7-130">Property</span></span>|<span data-ttu-id="1dae7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dae7-131">Type</span></span>|<span data-ttu-id="1dae7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dae7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dae7-133">id</span><span class="sxs-lookup"><span data-stu-id="1dae7-133">id</span></span>|<span data-ttu-id="1dae7-134">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-134">String</span></span>|<span data-ttu-id="1dae7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1dae7-135">Key of the entity.</span></span> <span data-ttu-id="1dae7-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1dae7-137">displayName</span></span>|<span data-ttu-id="1dae7-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dae7-138">String</span></span>|<span data-ttu-id="1dae7-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1dae7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1dae7-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-141">description</span><span class="sxs-lookup"><span data-stu-id="1dae7-141">description</span></span>|<span data-ttu-id="1dae7-142">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-142">String</span></span>|<span data-ttu-id="1dae7-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dae7-143">The description of the app.</span></span> <span data-ttu-id="1dae7-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-145">publicador</span><span class="sxs-lookup"><span data-stu-id="1dae7-145">publisher</span></span>|<span data-ttu-id="1dae7-146">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-146">String</span></span>|<span data-ttu-id="1dae7-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dae7-147">The publisher of the app.</span></span> <span data-ttu-id="1dae7-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1dae7-149">largeIcon</span></span>|[<span data-ttu-id="1dae7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1dae7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1dae7-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1dae7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1dae7-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1dae7-153">createdDateTime</span></span>|<span data-ttu-id="1dae7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dae7-154">DateTimeOffset</span></span>|<span data-ttu-id="1dae7-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dae7-155">The date and time the app was created.</span></span> <span data-ttu-id="1dae7-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dae7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1dae7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dae7-158">DateTimeOffset</span></span>|<span data-ttu-id="1dae7-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1dae7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1dae7-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1dae7-161">isFeatured</span></span>|<span data-ttu-id="1dae7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dae7-162">Boolean</span></span>|<span data-ttu-id="1dae7-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1dae7-164">privacyInformationUrl</span></span>|<span data-ttu-id="1dae7-165">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-165">String</span></span>|<span data-ttu-id="1dae7-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1dae7-166">The privacy statement Url.</span></span> <span data-ttu-id="1dae7-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1dae7-168">informationUrl</span></span>|<span data-ttu-id="1dae7-169">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-169">String</span></span>|<span data-ttu-id="1dae7-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1dae7-170">The more information Url.</span></span> <span data-ttu-id="1dae7-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-172">owner</span><span class="sxs-lookup"><span data-stu-id="1dae7-172">owner</span></span>|<span data-ttu-id="1dae7-173">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-173">String</span></span>|<span data-ttu-id="1dae7-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1dae7-174">The owner of the app.</span></span> <span data-ttu-id="1dae7-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-176">developer</span><span class="sxs-lookup"><span data-stu-id="1dae7-176">developer</span></span>|<span data-ttu-id="1dae7-177">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-177">String</span></span>|<span data-ttu-id="1dae7-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dae7-178">The developer of the app.</span></span> <span data-ttu-id="1dae7-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-180">notes</span><span class="sxs-lookup"><span data-stu-id="1dae7-180">notes</span></span>|<span data-ttu-id="1dae7-181">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-181">String</span></span>|<span data-ttu-id="1dae7-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dae7-182">Notes for the app.</span></span> <span data-ttu-id="1dae7-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1dae7-184">uploadState</span></span>|<span data-ttu-id="1dae7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae7-185">Int32</span></span>|<span data-ttu-id="1dae7-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="1dae7-186">The upload state.</span></span> <span data-ttu-id="1dae7-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1dae7-188">publishingState</span></span>|[<span data-ttu-id="1dae7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1dae7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1dae7-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dae7-190">The publishing state for the app.</span></span> <span data-ttu-id="1dae7-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1dae7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1dae7-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1dae7-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1dae7-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1dae7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1dae7-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1dae7-194">isAssigned</span></span>|<span data-ttu-id="1dae7-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dae7-195">Boolean</span></span>|<span data-ttu-id="1dae7-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="1dae7-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1dae7-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1dae7-198">roleScopeTagIds</span></span>|<span data-ttu-id="1dae7-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1dae7-199">String collection</span></span>|<span data-ttu-id="1dae7-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="1dae7-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1dae7-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="1dae7-202">dependentAppCount</span></span>|<span data-ttu-id="1dae7-203">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae7-203">Int32</span></span>|<span data-ttu-id="1dae7-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="1dae7-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1dae7-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1dae7-206">packageId</span><span class="sxs-lookup"><span data-stu-id="1dae7-206">packageId</span></span>|<span data-ttu-id="1dae7-207">String</span><span class="sxs-lookup"><span data-stu-id="1dae7-207">String</span></span>|<span data-ttu-id="1dae7-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="1dae7-208">The package identifier.</span></span> <span data-ttu-id="1dae7-209">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-209">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="1dae7-210">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="1dae7-210">appIdentifier</span></span>|<span data-ttu-id="1dae7-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dae7-211">String</span></span>|<span data-ttu-id="1dae7-212">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1dae7-212">The Identity Name.</span></span> <span data-ttu-id="1dae7-213">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-213">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="1dae7-214">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1dae7-214">usedLicenseCount</span></span>|<span data-ttu-id="1dae7-215">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae7-215">Int32</span></span>|<span data-ttu-id="1dae7-216">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="1dae7-216">The number of VPP licenses in use.</span></span> <span data-ttu-id="1dae7-217">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-217">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="1dae7-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1dae7-218">totalLicenseCount</span></span>|<span data-ttu-id="1dae7-219">Int32</span><span class="sxs-lookup"><span data-stu-id="1dae7-219">Int32</span></span>|<span data-ttu-id="1dae7-220">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="1dae7-220">The total number of VPP licenses.</span></span> <span data-ttu-id="1dae7-221">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-221">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="1dae7-222">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1dae7-222">appStoreUrl</span></span>|<span data-ttu-id="1dae7-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dae7-223">String</span></span>|<span data-ttu-id="1dae7-224">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1dae7-224">The Play for Work Store app URL.</span></span> <span data-ttu-id="1dae7-225">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-225">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="1dae7-226">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="1dae7-226">isPrivate</span></span>|<span data-ttu-id="1dae7-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dae7-227">Boolean</span></span>|<span data-ttu-id="1dae7-228">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="1dae7-228">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="1dae7-229">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-229">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="1dae7-230">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="1dae7-230">isSystemApp</span></span>|<span data-ttu-id="1dae7-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dae7-231">Boolean</span></span>|<span data-ttu-id="1dae7-232">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="1dae7-232">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="1dae7-233">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-233">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="1dae7-234">appTracks</span><span class="sxs-lookup"><span data-stu-id="1dae7-234">appTracks</span></span>|<span data-ttu-id="1dae7-235">coleção [androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-235">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="1dae7-236">As faixas que são visíveis para esta empresa.</span><span class="sxs-lookup"><span data-stu-id="1dae7-236">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="1dae7-237">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-237">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="1dae7-238">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="1dae7-238">supportsOemConfig</span></span>|<span data-ttu-id="1dae7-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dae7-239">Boolean</span></span>|<span data-ttu-id="1dae7-240">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="1dae7-240">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="1dae7-241">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dae7-241">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1dae7-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dae7-242">Response</span></span>
<span data-ttu-id="1dae7-243">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dae7-243">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dae7-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dae7-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dae7-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dae7-245">Request</span></span>
<span data-ttu-id="1dae7-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dae7-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1171

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="1dae7-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dae7-247">Response</span></span>
<span data-ttu-id="1dae7-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dae7-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1343

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
  "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```



