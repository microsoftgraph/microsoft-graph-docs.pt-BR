---
title: Atualizar androidManagedStoreWebApp
description: Atualiza as propriedades de um objeto androidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 546ce711d688297a694a5a210f53f466573ff93f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253253"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="592ff-103">Atualizar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="592ff-103">Update androidManagedStoreWebApp</span></span>

<span data-ttu-id="592ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="592ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="592ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="592ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="592ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="592ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="592ff-107">Atualiza as propriedades de um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="592ff-107">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="592ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="592ff-108">Prerequisites</span></span>
<span data-ttu-id="592ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="592ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="592ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="592ff-111">Permission type</span></span>|<span data-ttu-id="592ff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="592ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="592ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="592ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="592ff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="592ff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="592ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="592ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="592ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="592ff-116">Not supported.</span></span>|
|<span data-ttu-id="592ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="592ff-117">Application</span></span>|<span data-ttu-id="592ff-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="592ff-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="592ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="592ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="592ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="592ff-120">Request headers</span></span>
|<span data-ttu-id="592ff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="592ff-121">Header</span></span>|<span data-ttu-id="592ff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="592ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="592ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="592ff-123">Authorization</span></span>|<span data-ttu-id="592ff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="592ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="592ff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="592ff-125">Accept</span></span>|<span data-ttu-id="592ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="592ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="592ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="592ff-127">Request body</span></span>
<span data-ttu-id="592ff-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="592ff-128">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="592ff-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span><span class="sxs-lookup"><span data-stu-id="592ff-129">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="592ff-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="592ff-130">Property</span></span>|<span data-ttu-id="592ff-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="592ff-131">Type</span></span>|<span data-ttu-id="592ff-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="592ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="592ff-133">id</span><span class="sxs-lookup"><span data-stu-id="592ff-133">id</span></span>|<span data-ttu-id="592ff-134">String</span><span class="sxs-lookup"><span data-stu-id="592ff-134">String</span></span>|<span data-ttu-id="592ff-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="592ff-135">Key of the entity.</span></span> <span data-ttu-id="592ff-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-137">displayName</span><span class="sxs-lookup"><span data-stu-id="592ff-137">displayName</span></span>|<span data-ttu-id="592ff-138">String</span><span class="sxs-lookup"><span data-stu-id="592ff-138">String</span></span>|<span data-ttu-id="592ff-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="592ff-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="592ff-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-141">description</span><span class="sxs-lookup"><span data-stu-id="592ff-141">description</span></span>|<span data-ttu-id="592ff-142">String</span><span class="sxs-lookup"><span data-stu-id="592ff-142">String</span></span>|<span data-ttu-id="592ff-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="592ff-143">The description of the app.</span></span> <span data-ttu-id="592ff-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-145">publicador</span><span class="sxs-lookup"><span data-stu-id="592ff-145">publisher</span></span>|<span data-ttu-id="592ff-146">String</span><span class="sxs-lookup"><span data-stu-id="592ff-146">String</span></span>|<span data-ttu-id="592ff-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="592ff-147">The publisher of the app.</span></span> <span data-ttu-id="592ff-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="592ff-149">largeIcon</span></span>|[<span data-ttu-id="592ff-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="592ff-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="592ff-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="592ff-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="592ff-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="592ff-153">createdDateTime</span></span>|<span data-ttu-id="592ff-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="592ff-154">DateTimeOffset</span></span>|<span data-ttu-id="592ff-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="592ff-155">The date and time the app was created.</span></span> <span data-ttu-id="592ff-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="592ff-157">lastModifiedDateTime</span></span>|<span data-ttu-id="592ff-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="592ff-158">DateTimeOffset</span></span>|<span data-ttu-id="592ff-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="592ff-159">The date and time the app was last modified.</span></span> <span data-ttu-id="592ff-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="592ff-161">isFeatured</span></span>|<span data-ttu-id="592ff-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="592ff-162">Boolean</span></span>|<span data-ttu-id="592ff-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="592ff-164">privacyInformationUrl</span></span>|<span data-ttu-id="592ff-165">String</span><span class="sxs-lookup"><span data-stu-id="592ff-165">String</span></span>|<span data-ttu-id="592ff-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="592ff-166">The privacy statement Url.</span></span> <span data-ttu-id="592ff-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="592ff-168">informationUrl</span></span>|<span data-ttu-id="592ff-169">String</span><span class="sxs-lookup"><span data-stu-id="592ff-169">String</span></span>|<span data-ttu-id="592ff-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="592ff-170">The more information Url.</span></span> <span data-ttu-id="592ff-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-172">owner</span><span class="sxs-lookup"><span data-stu-id="592ff-172">owner</span></span>|<span data-ttu-id="592ff-173">String</span><span class="sxs-lookup"><span data-stu-id="592ff-173">String</span></span>|<span data-ttu-id="592ff-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="592ff-174">The owner of the app.</span></span> <span data-ttu-id="592ff-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-176">developer</span><span class="sxs-lookup"><span data-stu-id="592ff-176">developer</span></span>|<span data-ttu-id="592ff-177">String</span><span class="sxs-lookup"><span data-stu-id="592ff-177">String</span></span>|<span data-ttu-id="592ff-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="592ff-178">The developer of the app.</span></span> <span data-ttu-id="592ff-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-180">notes</span><span class="sxs-lookup"><span data-stu-id="592ff-180">notes</span></span>|<span data-ttu-id="592ff-181">String</span><span class="sxs-lookup"><span data-stu-id="592ff-181">String</span></span>|<span data-ttu-id="592ff-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="592ff-182">Notes for the app.</span></span> <span data-ttu-id="592ff-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="592ff-184">uploadState</span></span>|<span data-ttu-id="592ff-185">Int32</span><span class="sxs-lookup"><span data-stu-id="592ff-185">Int32</span></span>|<span data-ttu-id="592ff-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="592ff-186">The upload state.</span></span> <span data-ttu-id="592ff-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="592ff-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="592ff-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="592ff-189">publishingState</span></span>|[<span data-ttu-id="592ff-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="592ff-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="592ff-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="592ff-191">The publishing state for the app.</span></span> <span data-ttu-id="592ff-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="592ff-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="592ff-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="592ff-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="592ff-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="592ff-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="592ff-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="592ff-195">isAssigned</span></span>|<span data-ttu-id="592ff-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="592ff-196">Boolean</span></span>|<span data-ttu-id="592ff-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="592ff-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="592ff-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="592ff-199">roleScopeTagIds</span></span>|<span data-ttu-id="592ff-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="592ff-200">String collection</span></span>|<span data-ttu-id="592ff-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="592ff-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="592ff-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="592ff-203">dependentAppCount</span></span>|<span data-ttu-id="592ff-204">Int32</span><span class="sxs-lookup"><span data-stu-id="592ff-204">Int32</span></span>|<span data-ttu-id="592ff-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="592ff-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="592ff-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="592ff-207">supersedingAppCount</span></span>|<span data-ttu-id="592ff-208">Int32</span><span class="sxs-lookup"><span data-stu-id="592ff-208">Int32</span></span>|<span data-ttu-id="592ff-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="592ff-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="592ff-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="592ff-211">supersededAppCount</span></span>|<span data-ttu-id="592ff-212">Int32</span><span class="sxs-lookup"><span data-stu-id="592ff-212">Int32</span></span>|<span data-ttu-id="592ff-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="592ff-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="592ff-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="592ff-215">packageId</span><span class="sxs-lookup"><span data-stu-id="592ff-215">packageId</span></span>|<span data-ttu-id="592ff-216">String</span><span class="sxs-lookup"><span data-stu-id="592ff-216">String</span></span>|<span data-ttu-id="592ff-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="592ff-217">The package identifier.</span></span> <span data-ttu-id="592ff-218">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="592ff-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="592ff-219">appIdentifier</span></span>|<span data-ttu-id="592ff-220">String</span><span class="sxs-lookup"><span data-stu-id="592ff-220">String</span></span>|<span data-ttu-id="592ff-221">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="592ff-221">The Identity Name.</span></span> <span data-ttu-id="592ff-222">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="592ff-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="592ff-223">usedLicenseCount</span></span>|<span data-ttu-id="592ff-224">Int32</span><span class="sxs-lookup"><span data-stu-id="592ff-224">Int32</span></span>|<span data-ttu-id="592ff-225">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="592ff-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="592ff-226">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="592ff-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="592ff-227">totalLicenseCount</span></span>|<span data-ttu-id="592ff-228">Int32</span><span class="sxs-lookup"><span data-stu-id="592ff-228">Int32</span></span>|<span data-ttu-id="592ff-229">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="592ff-229">The total number of VPP licenses.</span></span> <span data-ttu-id="592ff-230">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="592ff-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="592ff-231">appStoreUrl</span></span>|<span data-ttu-id="592ff-232">String</span><span class="sxs-lookup"><span data-stu-id="592ff-232">String</span></span>|<span data-ttu-id="592ff-233">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="592ff-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="592ff-234">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="592ff-235">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="592ff-235">isPrivate</span></span>|<span data-ttu-id="592ff-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="592ff-236">Boolean</span></span>|<span data-ttu-id="592ff-237">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="592ff-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="592ff-238">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="592ff-239">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="592ff-239">isSystemApp</span></span>|<span data-ttu-id="592ff-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="592ff-240">Boolean</span></span>|<span data-ttu-id="592ff-241">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="592ff-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="592ff-242">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="592ff-243">appTracks</span><span class="sxs-lookup"><span data-stu-id="592ff-243">appTracks</span></span>|<span data-ttu-id="592ff-244">coleção [androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="592ff-245">As faixas que são visíveis para esta empresa.</span><span class="sxs-lookup"><span data-stu-id="592ff-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="592ff-246">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="592ff-247">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="592ff-247">supportsOemConfig</span></span>|<span data-ttu-id="592ff-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="592ff-248">Boolean</span></span>|<span data-ttu-id="592ff-249">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="592ff-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="592ff-250">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="592ff-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="592ff-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="592ff-251">Response</span></span>
<span data-ttu-id="592ff-252">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="592ff-252">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="592ff-253">Exemplo</span><span class="sxs-lookup"><span data-stu-id="592ff-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="592ff-254">Solicitação</span><span class="sxs-lookup"><span data-stu-id="592ff-254">Request</span></span>
<span data-ttu-id="592ff-255">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="592ff-255">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="592ff-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="592ff-256">Response</span></span>
<span data-ttu-id="592ff-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="592ff-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




