---
title: Atualizar androidManagedStoreWebApp
description: Atualize as propriedades de um objeto androidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11a011e018211d706f0dd340ac5a32137f2ea55f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144365"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="6c8e6-103">Atualizar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="6c8e6-103">Update androidManagedStoreWebApp</span></span>

<span data-ttu-id="6c8e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c8e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c8e6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c8e6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c8e6-107">Atualize as propriedades de um [objeto androidManagedStoreWebApp.](../resources/intune-apps-androidmanagedstorewebapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-107">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c8e6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c8e6-108">Prerequisites</span></span>
<span data-ttu-id="6c8e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c8e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c8e6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c8e6-111">Permission type</span></span>|<span data-ttu-id="6c8e6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c8e6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c8e6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c8e6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c8e6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c8e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-116">Not supported.</span></span>|
|<span data-ttu-id="6c8e6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c8e6-117">Application</span></span>|<span data-ttu-id="6c8e6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c8e6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c8e6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c8e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6c8e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c8e6-120">Request headers</span></span>
|<span data-ttu-id="6c8e6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c8e6-121">Header</span></span>|<span data-ttu-id="6c8e6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6c8e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c8e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c8e6-123">Authorization</span></span>|<span data-ttu-id="6c8e6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c8e6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c8e6-125">Accept</span></span>|<span data-ttu-id="6c8e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c8e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c8e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c8e6-127">Request body</span></span>
<span data-ttu-id="6c8e6-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidManagedStoreWebApp.](../resources/intune-apps-androidmanagedstorewebapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-128">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="6c8e6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c8e6-129">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="6c8e6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c8e6-130">Property</span></span>|<span data-ttu-id="6c8e6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c8e6-131">Type</span></span>|<span data-ttu-id="6c8e6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c8e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c8e6-133">id</span><span class="sxs-lookup"><span data-stu-id="6c8e6-133">id</span></span>|<span data-ttu-id="6c8e6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c8e6-134">String</span></span>|<span data-ttu-id="6c8e6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-135">Key of the entity.</span></span> <span data-ttu-id="6c8e6-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6c8e6-137">displayName</span></span>|<span data-ttu-id="6c8e6-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c8e6-138">String</span></span>|<span data-ttu-id="6c8e6-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6c8e6-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-141">descrição</span><span class="sxs-lookup"><span data-stu-id="6c8e6-141">description</span></span>|<span data-ttu-id="6c8e6-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c8e6-142">String</span></span>|<span data-ttu-id="6c8e6-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-143">The description of the app.</span></span> <span data-ttu-id="6c8e6-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-145">publicador</span><span class="sxs-lookup"><span data-stu-id="6c8e6-145">publisher</span></span>|<span data-ttu-id="6c8e6-146">String</span><span class="sxs-lookup"><span data-stu-id="6c8e6-146">String</span></span>|<span data-ttu-id="6c8e6-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-147">The publisher of the app.</span></span> <span data-ttu-id="6c8e6-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6c8e6-149">largeIcon</span></span>|[<span data-ttu-id="6c8e6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6c8e6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6c8e6-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6c8e6-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c8e6-153">createdDateTime</span></span>|<span data-ttu-id="6c8e6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c8e6-154">DateTimeOffset</span></span>|<span data-ttu-id="6c8e6-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-155">The date and time the app was created.</span></span> <span data-ttu-id="6c8e6-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c8e6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6c8e6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c8e6-158">DateTimeOffset</span></span>|<span data-ttu-id="6c8e6-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6c8e6-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6c8e6-161">isFeatured</span></span>|<span data-ttu-id="6c8e6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8e6-162">Boolean</span></span>|<span data-ttu-id="6c8e6-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6c8e6-164">privacyInformationUrl</span></span>|<span data-ttu-id="6c8e6-165">String</span><span class="sxs-lookup"><span data-stu-id="6c8e6-165">String</span></span>|<span data-ttu-id="6c8e6-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-166">The privacy statement Url.</span></span> <span data-ttu-id="6c8e6-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6c8e6-168">informationUrl</span></span>|<span data-ttu-id="6c8e6-169">String</span><span class="sxs-lookup"><span data-stu-id="6c8e6-169">String</span></span>|<span data-ttu-id="6c8e6-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-170">The more information Url.</span></span> <span data-ttu-id="6c8e6-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-172">owner</span><span class="sxs-lookup"><span data-stu-id="6c8e6-172">owner</span></span>|<span data-ttu-id="6c8e6-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c8e6-173">String</span></span>|<span data-ttu-id="6c8e6-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-174">The owner of the app.</span></span> <span data-ttu-id="6c8e6-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-176">developer</span><span class="sxs-lookup"><span data-stu-id="6c8e6-176">developer</span></span>|<span data-ttu-id="6c8e6-177">String</span><span class="sxs-lookup"><span data-stu-id="6c8e6-177">String</span></span>|<span data-ttu-id="6c8e6-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-178">The developer of the app.</span></span> <span data-ttu-id="6c8e6-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-180">notes</span><span class="sxs-lookup"><span data-stu-id="6c8e6-180">notes</span></span>|<span data-ttu-id="6c8e6-181">String</span><span class="sxs-lookup"><span data-stu-id="6c8e6-181">String</span></span>|<span data-ttu-id="6c8e6-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-182">Notes for the app.</span></span> <span data-ttu-id="6c8e6-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6c8e6-184">uploadState</span></span>|<span data-ttu-id="6c8e6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6c8e6-185">Int32</span></span>|<span data-ttu-id="6c8e6-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-186">The upload state.</span></span> <span data-ttu-id="6c8e6-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="6c8e6-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="6c8e6-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="6c8e6-189">publishingState</span></span>|[<span data-ttu-id="6c8e6-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6c8e6-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6c8e6-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-191">The publishing state for the app.</span></span> <span data-ttu-id="6c8e6-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6c8e6-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c8e6-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6c8e6-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6c8e6-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6c8e6-195">isAssigned</span></span>|<span data-ttu-id="6c8e6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c8e6-196">Boolean</span></span>|<span data-ttu-id="6c8e6-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6c8e6-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c8e6-199">roleScopeTagIds</span></span>|<span data-ttu-id="6c8e6-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c8e6-200">String collection</span></span>|<span data-ttu-id="6c8e6-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6c8e6-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6c8e6-203">dependentAppCount</span></span>|<span data-ttu-id="6c8e6-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6c8e6-204">Int32</span></span>|<span data-ttu-id="6c8e6-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6c8e6-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="6c8e6-207">supersedingAppCount</span></span>|<span data-ttu-id="6c8e6-208">Int32</span><span class="sxs-lookup"><span data-stu-id="6c8e6-208">Int32</span></span>|<span data-ttu-id="6c8e6-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="6c8e6-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="6c8e6-211">supersededAppCount</span></span>|<span data-ttu-id="6c8e6-212">Int32</span><span class="sxs-lookup"><span data-stu-id="6c8e6-212">Int32</span></span>|<span data-ttu-id="6c8e6-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="6c8e6-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c8e6-215">packageId</span><span class="sxs-lookup"><span data-stu-id="6c8e6-215">packageId</span></span>|<span data-ttu-id="6c8e6-216">String</span><span class="sxs-lookup"><span data-stu-id="6c8e6-216">String</span></span>|<span data-ttu-id="6c8e6-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-217">The package identifier.</span></span> <span data-ttu-id="6c8e6-218">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6c8e6-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6c8e6-219">appIdentifier</span></span>|<span data-ttu-id="6c8e6-220">String</span><span class="sxs-lookup"><span data-stu-id="6c8e6-220">String</span></span>|<span data-ttu-id="6c8e6-221">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-221">The Identity Name.</span></span> <span data-ttu-id="6c8e6-222">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6c8e6-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6c8e6-223">usedLicenseCount</span></span>|<span data-ttu-id="6c8e6-224">Int32</span><span class="sxs-lookup"><span data-stu-id="6c8e6-224">Int32</span></span>|<span data-ttu-id="6c8e6-225">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="6c8e6-226">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6c8e6-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6c8e6-227">totalLicenseCount</span></span>|<span data-ttu-id="6c8e6-228">Int32</span><span class="sxs-lookup"><span data-stu-id="6c8e6-228">Int32</span></span>|<span data-ttu-id="6c8e6-229">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-229">The total number of VPP licenses.</span></span> <span data-ttu-id="6c8e6-230">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6c8e6-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6c8e6-231">appStoreUrl</span></span>|<span data-ttu-id="6c8e6-232">String</span><span class="sxs-lookup"><span data-stu-id="6c8e6-232">String</span></span>|<span data-ttu-id="6c8e6-233">A URL do aplicativo Play for Work Store.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="6c8e6-234">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6c8e6-235">isPrivate</span><span class="sxs-lookup"><span data-stu-id="6c8e6-235">isPrivate</span></span>|<span data-ttu-id="6c8e6-236">Booleano</span><span class="sxs-lookup"><span data-stu-id="6c8e6-236">Boolean</span></span>|<span data-ttu-id="6c8e6-237">Indica se o aplicativo só está disponível para usuários de uma determinada empresa.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="6c8e6-238">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6c8e6-239">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="6c8e6-239">isSystemApp</span></span>|<span data-ttu-id="6c8e6-240">Booleano</span><span class="sxs-lookup"><span data-stu-id="6c8e6-240">Boolean</span></span>|<span data-ttu-id="6c8e6-241">Indica se o aplicativo é um aplicativo do sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="6c8e6-242">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6c8e6-243">appTracks</span><span class="sxs-lookup"><span data-stu-id="6c8e6-243">appTracks</span></span>|<span data-ttu-id="6c8e6-244">[Coleção androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="6c8e6-245">As faixas que estão visíveis para essa empresa.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="6c8e6-246">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6c8e6-247">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="6c8e6-247">supportsOemConfig</span></span>|<span data-ttu-id="6c8e6-248">Booleano</span><span class="sxs-lookup"><span data-stu-id="6c8e6-248">Boolean</span></span>|<span data-ttu-id="6c8e6-249">Se esse aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="6c8e6-250">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c8e6-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6c8e6-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c8e6-251">Response</span></span>
<span data-ttu-id="6c8e6-252">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-252">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c8e6-253">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c8e6-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c8e6-254">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c8e6-254">Request</span></span>
<span data-ttu-id="6c8e6-255">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-255">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1228

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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

### <a name="response"></a><span data-ttu-id="6c8e6-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c8e6-256">Response</span></span>
<span data-ttu-id="6c8e6-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c8e6-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1400

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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




