---
title: Criar androidManagedStoreWebApp
description: Crie um novo objeto androidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02c2ef44ea107529e40dd4a3f0d0ed0767f25979
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144379"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="12d90-103">Criar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="12d90-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="12d90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12d90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12d90-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12d90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12d90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12d90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12d90-107">Crie um novo [objeto androidManagedStoreWebApp.](../resources/intune-apps-androidmanagedstorewebapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12d90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12d90-108">Prerequisites</span></span>
<span data-ttu-id="12d90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12d90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12d90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12d90-111">Permission type</span></span>|<span data-ttu-id="12d90-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12d90-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12d90-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12d90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12d90-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12d90-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12d90-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12d90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12d90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12d90-116">Not supported.</span></span>|
|<span data-ttu-id="12d90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12d90-117">Application</span></span>|<span data-ttu-id="12d90-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12d90-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12d90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12d90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="12d90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12d90-120">Request headers</span></span>
|<span data-ttu-id="12d90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12d90-121">Header</span></span>|<span data-ttu-id="12d90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12d90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12d90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12d90-123">Authorization</span></span>|<span data-ttu-id="12d90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12d90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12d90-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12d90-125">Accept</span></span>|<span data-ttu-id="12d90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12d90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12d90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12d90-127">Request body</span></span>
<span data-ttu-id="12d90-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="12d90-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="12d90-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="12d90-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="12d90-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12d90-130">Property</span></span>|<span data-ttu-id="12d90-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="12d90-131">Type</span></span>|<span data-ttu-id="12d90-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="12d90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d90-133">id</span><span class="sxs-lookup"><span data-stu-id="12d90-133">id</span></span>|<span data-ttu-id="12d90-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12d90-134">String</span></span>|<span data-ttu-id="12d90-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="12d90-135">Key of the entity.</span></span> <span data-ttu-id="12d90-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-137">displayName</span><span class="sxs-lookup"><span data-stu-id="12d90-137">displayName</span></span>|<span data-ttu-id="12d90-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12d90-138">String</span></span>|<span data-ttu-id="12d90-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="12d90-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="12d90-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-141">descrição</span><span class="sxs-lookup"><span data-stu-id="12d90-141">description</span></span>|<span data-ttu-id="12d90-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12d90-142">String</span></span>|<span data-ttu-id="12d90-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d90-143">The description of the app.</span></span> <span data-ttu-id="12d90-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-145">publicador</span><span class="sxs-lookup"><span data-stu-id="12d90-145">publisher</span></span>|<span data-ttu-id="12d90-146">String</span><span class="sxs-lookup"><span data-stu-id="12d90-146">String</span></span>|<span data-ttu-id="12d90-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d90-147">The publisher of the app.</span></span> <span data-ttu-id="12d90-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="12d90-149">largeIcon</span></span>|[<span data-ttu-id="12d90-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="12d90-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="12d90-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="12d90-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="12d90-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12d90-153">createdDateTime</span></span>|<span data-ttu-id="12d90-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d90-154">DateTimeOffset</span></span>|<span data-ttu-id="12d90-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d90-155">The date and time the app was created.</span></span> <span data-ttu-id="12d90-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12d90-157">lastModifiedDateTime</span></span>|<span data-ttu-id="12d90-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d90-158">DateTimeOffset</span></span>|<span data-ttu-id="12d90-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="12d90-159">The date and time the app was last modified.</span></span> <span data-ttu-id="12d90-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="12d90-161">isFeatured</span></span>|<span data-ttu-id="12d90-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="12d90-162">Boolean</span></span>|<span data-ttu-id="12d90-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="12d90-164">privacyInformationUrl</span></span>|<span data-ttu-id="12d90-165">String</span><span class="sxs-lookup"><span data-stu-id="12d90-165">String</span></span>|<span data-ttu-id="12d90-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="12d90-166">The privacy statement Url.</span></span> <span data-ttu-id="12d90-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="12d90-168">informationUrl</span></span>|<span data-ttu-id="12d90-169">String</span><span class="sxs-lookup"><span data-stu-id="12d90-169">String</span></span>|<span data-ttu-id="12d90-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="12d90-170">The more information Url.</span></span> <span data-ttu-id="12d90-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-172">owner</span><span class="sxs-lookup"><span data-stu-id="12d90-172">owner</span></span>|<span data-ttu-id="12d90-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12d90-173">String</span></span>|<span data-ttu-id="12d90-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="12d90-174">The owner of the app.</span></span> <span data-ttu-id="12d90-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-176">developer</span><span class="sxs-lookup"><span data-stu-id="12d90-176">developer</span></span>|<span data-ttu-id="12d90-177">String</span><span class="sxs-lookup"><span data-stu-id="12d90-177">String</span></span>|<span data-ttu-id="12d90-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d90-178">The developer of the app.</span></span> <span data-ttu-id="12d90-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-180">notes</span><span class="sxs-lookup"><span data-stu-id="12d90-180">notes</span></span>|<span data-ttu-id="12d90-181">String</span><span class="sxs-lookup"><span data-stu-id="12d90-181">String</span></span>|<span data-ttu-id="12d90-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d90-182">Notes for the app.</span></span> <span data-ttu-id="12d90-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="12d90-184">uploadState</span></span>|<span data-ttu-id="12d90-185">Int32</span><span class="sxs-lookup"><span data-stu-id="12d90-185">Int32</span></span>|<span data-ttu-id="12d90-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="12d90-186">The upload state.</span></span> <span data-ttu-id="12d90-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="12d90-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="12d90-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="12d90-189">publishingState</span></span>|[<span data-ttu-id="12d90-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="12d90-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="12d90-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d90-191">The publishing state for the app.</span></span> <span data-ttu-id="12d90-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="12d90-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="12d90-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="12d90-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="12d90-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="12d90-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="12d90-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="12d90-195">isAssigned</span></span>|<span data-ttu-id="12d90-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="12d90-196">Boolean</span></span>|<span data-ttu-id="12d90-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="12d90-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="12d90-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12d90-199">roleScopeTagIds</span></span>|<span data-ttu-id="12d90-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="12d90-200">String collection</span></span>|<span data-ttu-id="12d90-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="12d90-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="12d90-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="12d90-203">dependentAppCount</span></span>|<span data-ttu-id="12d90-204">Int32</span><span class="sxs-lookup"><span data-stu-id="12d90-204">Int32</span></span>|<span data-ttu-id="12d90-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="12d90-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="12d90-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="12d90-207">supersedingAppCount</span></span>|<span data-ttu-id="12d90-208">Int32</span><span class="sxs-lookup"><span data-stu-id="12d90-208">Int32</span></span>|<span data-ttu-id="12d90-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="12d90-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="12d90-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="12d90-211">supersededAppCount</span></span>|<span data-ttu-id="12d90-212">Int32</span><span class="sxs-lookup"><span data-stu-id="12d90-212">Int32</span></span>|<span data-ttu-id="12d90-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="12d90-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="12d90-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d90-215">packageId</span><span class="sxs-lookup"><span data-stu-id="12d90-215">packageId</span></span>|<span data-ttu-id="12d90-216">String</span><span class="sxs-lookup"><span data-stu-id="12d90-216">String</span></span>|<span data-ttu-id="12d90-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="12d90-217">The package identifier.</span></span> <span data-ttu-id="12d90-218">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="12d90-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="12d90-219">appIdentifier</span></span>|<span data-ttu-id="12d90-220">String</span><span class="sxs-lookup"><span data-stu-id="12d90-220">String</span></span>|<span data-ttu-id="12d90-221">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="12d90-221">The Identity Name.</span></span> <span data-ttu-id="12d90-222">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="12d90-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="12d90-223">usedLicenseCount</span></span>|<span data-ttu-id="12d90-224">Int32</span><span class="sxs-lookup"><span data-stu-id="12d90-224">Int32</span></span>|<span data-ttu-id="12d90-225">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="12d90-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="12d90-226">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="12d90-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="12d90-227">totalLicenseCount</span></span>|<span data-ttu-id="12d90-228">Int32</span><span class="sxs-lookup"><span data-stu-id="12d90-228">Int32</span></span>|<span data-ttu-id="12d90-229">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="12d90-229">The total number of VPP licenses.</span></span> <span data-ttu-id="12d90-230">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="12d90-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="12d90-231">appStoreUrl</span></span>|<span data-ttu-id="12d90-232">String</span><span class="sxs-lookup"><span data-stu-id="12d90-232">String</span></span>|<span data-ttu-id="12d90-233">A URL do aplicativo Play for Work Store.</span><span class="sxs-lookup"><span data-stu-id="12d90-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="12d90-234">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="12d90-235">isPrivate</span><span class="sxs-lookup"><span data-stu-id="12d90-235">isPrivate</span></span>|<span data-ttu-id="12d90-236">Booleano</span><span class="sxs-lookup"><span data-stu-id="12d90-236">Boolean</span></span>|<span data-ttu-id="12d90-237">Indica se o aplicativo só está disponível para usuários de uma determinada empresa.</span><span class="sxs-lookup"><span data-stu-id="12d90-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="12d90-238">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="12d90-239">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="12d90-239">isSystemApp</span></span>|<span data-ttu-id="12d90-240">Booleano</span><span class="sxs-lookup"><span data-stu-id="12d90-240">Boolean</span></span>|<span data-ttu-id="12d90-241">Indica se o aplicativo é um aplicativo do sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="12d90-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="12d90-242">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="12d90-243">appTracks</span><span class="sxs-lookup"><span data-stu-id="12d90-243">appTracks</span></span>|<span data-ttu-id="12d90-244">[Coleção androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="12d90-245">As faixas que estão visíveis para essa empresa.</span><span class="sxs-lookup"><span data-stu-id="12d90-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="12d90-246">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="12d90-247">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="12d90-247">supportsOemConfig</span></span>|<span data-ttu-id="12d90-248">Booleano</span><span class="sxs-lookup"><span data-stu-id="12d90-248">Boolean</span></span>|<span data-ttu-id="12d90-249">Se esse aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="12d90-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="12d90-250">Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d90-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="12d90-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="12d90-251">Response</span></span>
<span data-ttu-id="12d90-252">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12d90-252">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12d90-253">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12d90-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="12d90-254">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12d90-254">Request</span></span>
<span data-ttu-id="12d90-255">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12d90-255">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="12d90-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="12d90-256">Response</span></span>
<span data-ttu-id="12d90-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12d90-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




