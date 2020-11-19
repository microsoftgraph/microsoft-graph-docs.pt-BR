---
title: Criar androidManagedStoreWebApp
description: Criar um novo objeto androidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 787dddb99654629296ae3274f479159d9da79cea
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253478"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="b996b-103">Criar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="b996b-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="b996b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b996b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b996b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b996b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b996b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b996b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b996b-107">Criar um novo objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b996b-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b996b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b996b-108">Prerequisites</span></span>
<span data-ttu-id="b996b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b996b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b996b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b996b-111">Permission type</span></span>|<span data-ttu-id="b996b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b996b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b996b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b996b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b996b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b996b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b996b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b996b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b996b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b996b-116">Not supported.</span></span>|
|<span data-ttu-id="b996b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b996b-117">Application</span></span>|<span data-ttu-id="b996b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b996b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b996b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b996b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b996b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b996b-120">Request headers</span></span>
|<span data-ttu-id="b996b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b996b-121">Header</span></span>|<span data-ttu-id="b996b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b996b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b996b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b996b-123">Authorization</span></span>|<span data-ttu-id="b996b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b996b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b996b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b996b-125">Accept</span></span>|<span data-ttu-id="b996b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b996b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b996b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b996b-127">Request body</span></span>
<span data-ttu-id="b996b-128">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="b996b-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="b996b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="b996b-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="b996b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b996b-130">Property</span></span>|<span data-ttu-id="b996b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b996b-131">Type</span></span>|<span data-ttu-id="b996b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b996b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b996b-133">id</span><span class="sxs-lookup"><span data-stu-id="b996b-133">id</span></span>|<span data-ttu-id="b996b-134">String</span><span class="sxs-lookup"><span data-stu-id="b996b-134">String</span></span>|<span data-ttu-id="b996b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b996b-135">Key of the entity.</span></span> <span data-ttu-id="b996b-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b996b-137">displayName</span></span>|<span data-ttu-id="b996b-138">String</span><span class="sxs-lookup"><span data-stu-id="b996b-138">String</span></span>|<span data-ttu-id="b996b-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b996b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b996b-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-141">description</span><span class="sxs-lookup"><span data-stu-id="b996b-141">description</span></span>|<span data-ttu-id="b996b-142">String</span><span class="sxs-lookup"><span data-stu-id="b996b-142">String</span></span>|<span data-ttu-id="b996b-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b996b-143">The description of the app.</span></span> <span data-ttu-id="b996b-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-145">publicador</span><span class="sxs-lookup"><span data-stu-id="b996b-145">publisher</span></span>|<span data-ttu-id="b996b-146">String</span><span class="sxs-lookup"><span data-stu-id="b996b-146">String</span></span>|<span data-ttu-id="b996b-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b996b-147">The publisher of the app.</span></span> <span data-ttu-id="b996b-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b996b-149">largeIcon</span></span>|[<span data-ttu-id="b996b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b996b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b996b-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b996b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b996b-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b996b-153">createdDateTime</span></span>|<span data-ttu-id="b996b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b996b-154">DateTimeOffset</span></span>|<span data-ttu-id="b996b-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b996b-155">The date and time the app was created.</span></span> <span data-ttu-id="b996b-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b996b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b996b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b996b-158">DateTimeOffset</span></span>|<span data-ttu-id="b996b-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b996b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b996b-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b996b-161">isFeatured</span></span>|<span data-ttu-id="b996b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b996b-162">Boolean</span></span>|<span data-ttu-id="b996b-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b996b-164">privacyInformationUrl</span></span>|<span data-ttu-id="b996b-165">String</span><span class="sxs-lookup"><span data-stu-id="b996b-165">String</span></span>|<span data-ttu-id="b996b-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b996b-166">The privacy statement Url.</span></span> <span data-ttu-id="b996b-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b996b-168">informationUrl</span></span>|<span data-ttu-id="b996b-169">String</span><span class="sxs-lookup"><span data-stu-id="b996b-169">String</span></span>|<span data-ttu-id="b996b-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b996b-170">The more information Url.</span></span> <span data-ttu-id="b996b-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-172">owner</span><span class="sxs-lookup"><span data-stu-id="b996b-172">owner</span></span>|<span data-ttu-id="b996b-173">String</span><span class="sxs-lookup"><span data-stu-id="b996b-173">String</span></span>|<span data-ttu-id="b996b-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b996b-174">The owner of the app.</span></span> <span data-ttu-id="b996b-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-176">developer</span><span class="sxs-lookup"><span data-stu-id="b996b-176">developer</span></span>|<span data-ttu-id="b996b-177">String</span><span class="sxs-lookup"><span data-stu-id="b996b-177">String</span></span>|<span data-ttu-id="b996b-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b996b-178">The developer of the app.</span></span> <span data-ttu-id="b996b-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-180">notes</span><span class="sxs-lookup"><span data-stu-id="b996b-180">notes</span></span>|<span data-ttu-id="b996b-181">String</span><span class="sxs-lookup"><span data-stu-id="b996b-181">String</span></span>|<span data-ttu-id="b996b-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b996b-182">Notes for the app.</span></span> <span data-ttu-id="b996b-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b996b-184">uploadState</span></span>|<span data-ttu-id="b996b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b996b-185">Int32</span></span>|<span data-ttu-id="b996b-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="b996b-186">The upload state.</span></span> <span data-ttu-id="b996b-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="b996b-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="b996b-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="b996b-189">publishingState</span></span>|[<span data-ttu-id="b996b-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b996b-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b996b-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b996b-191">The publishing state for the app.</span></span> <span data-ttu-id="b996b-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b996b-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b996b-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b996b-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b996b-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b996b-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b996b-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b996b-195">isAssigned</span></span>|<span data-ttu-id="b996b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b996b-196">Boolean</span></span>|<span data-ttu-id="b996b-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="b996b-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b996b-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b996b-199">roleScopeTagIds</span></span>|<span data-ttu-id="b996b-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b996b-200">String collection</span></span>|<span data-ttu-id="b996b-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b996b-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b996b-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b996b-203">dependentAppCount</span></span>|<span data-ttu-id="b996b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="b996b-204">Int32</span></span>|<span data-ttu-id="b996b-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="b996b-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b996b-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="b996b-207">supersedingAppCount</span></span>|<span data-ttu-id="b996b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="b996b-208">Int32</span></span>|<span data-ttu-id="b996b-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="b996b-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="b996b-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="b996b-211">supersededAppCount</span></span>|<span data-ttu-id="b996b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b996b-212">Int32</span></span>|<span data-ttu-id="b996b-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="b996b-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="b996b-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b996b-215">packageId</span><span class="sxs-lookup"><span data-stu-id="b996b-215">packageId</span></span>|<span data-ttu-id="b996b-216">String</span><span class="sxs-lookup"><span data-stu-id="b996b-216">String</span></span>|<span data-ttu-id="b996b-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="b996b-217">The package identifier.</span></span> <span data-ttu-id="b996b-218">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="b996b-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="b996b-219">appIdentifier</span></span>|<span data-ttu-id="b996b-220">String</span><span class="sxs-lookup"><span data-stu-id="b996b-220">String</span></span>|<span data-ttu-id="b996b-221">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b996b-221">The Identity Name.</span></span> <span data-ttu-id="b996b-222">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="b996b-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b996b-223">usedLicenseCount</span></span>|<span data-ttu-id="b996b-224">Int32</span><span class="sxs-lookup"><span data-stu-id="b996b-224">Int32</span></span>|<span data-ttu-id="b996b-225">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="b996b-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="b996b-226">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="b996b-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b996b-227">totalLicenseCount</span></span>|<span data-ttu-id="b996b-228">Int32</span><span class="sxs-lookup"><span data-stu-id="b996b-228">Int32</span></span>|<span data-ttu-id="b996b-229">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="b996b-229">The total number of VPP licenses.</span></span> <span data-ttu-id="b996b-230">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="b996b-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b996b-231">appStoreUrl</span></span>|<span data-ttu-id="b996b-232">String</span><span class="sxs-lookup"><span data-stu-id="b996b-232">String</span></span>|<span data-ttu-id="b996b-233">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b996b-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="b996b-234">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="b996b-235">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="b996b-235">isPrivate</span></span>|<span data-ttu-id="b996b-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="b996b-236">Boolean</span></span>|<span data-ttu-id="b996b-237">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="b996b-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="b996b-238">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="b996b-239">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="b996b-239">isSystemApp</span></span>|<span data-ttu-id="b996b-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="b996b-240">Boolean</span></span>|<span data-ttu-id="b996b-241">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="b996b-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="b996b-242">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="b996b-243">appTracks</span><span class="sxs-lookup"><span data-stu-id="b996b-243">appTracks</span></span>|<span data-ttu-id="b996b-244">coleção [androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="b996b-245">As faixas que são visíveis para esta empresa.</span><span class="sxs-lookup"><span data-stu-id="b996b-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="b996b-246">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="b996b-247">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="b996b-247">supportsOemConfig</span></span>|<span data-ttu-id="b996b-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="b996b-248">Boolean</span></span>|<span data-ttu-id="b996b-249">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="b996b-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="b996b-250">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="b996b-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b996b-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="b996b-251">Response</span></span>
<span data-ttu-id="b996b-252">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b996b-252">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b996b-253">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b996b-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="b996b-254">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b996b-254">Request</span></span>
<span data-ttu-id="b996b-255">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b996b-255">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b996b-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="b996b-256">Response</span></span>
<span data-ttu-id="b996b-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b996b-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




