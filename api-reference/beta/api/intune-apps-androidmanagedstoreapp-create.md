---
title: Criar androidManagedStoreApp
description: Crie um novo objeto androidManagedStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61381599a4de67e5b4b691d22364cd82737d9adc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144435"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="8d7bc-103">Criar androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="8d7bc-103">Create androidManagedStoreApp</span></span>

<span data-ttu-id="8d7bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d7bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d7bc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d7bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d7bc-107">Crie um novo [objeto androidManagedStoreApp.](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-107">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d7bc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d7bc-108">Prerequisites</span></span>
<span data-ttu-id="8d7bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d7bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d7bc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d7bc-111">Permission type</span></span>|<span data-ttu-id="8d7bc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d7bc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d7bc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d7bc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d7bc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d7bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-116">Not supported.</span></span>|
|<span data-ttu-id="8d7bc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d7bc-117">Application</span></span>|<span data-ttu-id="8d7bc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d7bc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d7bc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d7bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8d7bc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d7bc-120">Request headers</span></span>
|<span data-ttu-id="8d7bc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d7bc-121">Header</span></span>|<span data-ttu-id="8d7bc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8d7bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d7bc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d7bc-123">Authorization</span></span>|<span data-ttu-id="8d7bc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d7bc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d7bc-125">Accept</span></span>|<span data-ttu-id="8d7bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d7bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d7bc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d7bc-127">Request body</span></span>
<span data-ttu-id="8d7bc-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-128">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="8d7bc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-129">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="8d7bc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d7bc-130">Property</span></span>|<span data-ttu-id="8d7bc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d7bc-131">Type</span></span>|<span data-ttu-id="8d7bc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d7bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d7bc-133">id</span><span class="sxs-lookup"><span data-stu-id="8d7bc-133">id</span></span>|<span data-ttu-id="8d7bc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d7bc-134">String</span></span>|<span data-ttu-id="8d7bc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-135">Key of the entity.</span></span> <span data-ttu-id="8d7bc-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8d7bc-137">displayName</span></span>|<span data-ttu-id="8d7bc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d7bc-138">String</span></span>|<span data-ttu-id="8d7bc-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8d7bc-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-141">descrição</span><span class="sxs-lookup"><span data-stu-id="8d7bc-141">description</span></span>|<span data-ttu-id="8d7bc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d7bc-142">String</span></span>|<span data-ttu-id="8d7bc-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-143">The description of the app.</span></span> <span data-ttu-id="8d7bc-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-145">publicador</span><span class="sxs-lookup"><span data-stu-id="8d7bc-145">publisher</span></span>|<span data-ttu-id="8d7bc-146">String</span><span class="sxs-lookup"><span data-stu-id="8d7bc-146">String</span></span>|<span data-ttu-id="8d7bc-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-147">The publisher of the app.</span></span> <span data-ttu-id="8d7bc-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8d7bc-149">largeIcon</span></span>|[<span data-ttu-id="8d7bc-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8d7bc-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8d7bc-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8d7bc-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d7bc-153">createdDateTime</span></span>|<span data-ttu-id="8d7bc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d7bc-154">DateTimeOffset</span></span>|<span data-ttu-id="8d7bc-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-155">The date and time the app was created.</span></span> <span data-ttu-id="8d7bc-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d7bc-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8d7bc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d7bc-158">DateTimeOffset</span></span>|<span data-ttu-id="8d7bc-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8d7bc-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8d7bc-161">isFeatured</span></span>|<span data-ttu-id="8d7bc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d7bc-162">Boolean</span></span>|<span data-ttu-id="8d7bc-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8d7bc-164">privacyInformationUrl</span></span>|<span data-ttu-id="8d7bc-165">String</span><span class="sxs-lookup"><span data-stu-id="8d7bc-165">String</span></span>|<span data-ttu-id="8d7bc-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-166">The privacy statement Url.</span></span> <span data-ttu-id="8d7bc-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8d7bc-168">informationUrl</span></span>|<span data-ttu-id="8d7bc-169">String</span><span class="sxs-lookup"><span data-stu-id="8d7bc-169">String</span></span>|<span data-ttu-id="8d7bc-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-170">The more information Url.</span></span> <span data-ttu-id="8d7bc-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-172">owner</span><span class="sxs-lookup"><span data-stu-id="8d7bc-172">owner</span></span>|<span data-ttu-id="8d7bc-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d7bc-173">String</span></span>|<span data-ttu-id="8d7bc-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-174">The owner of the app.</span></span> <span data-ttu-id="8d7bc-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-176">developer</span><span class="sxs-lookup"><span data-stu-id="8d7bc-176">developer</span></span>|<span data-ttu-id="8d7bc-177">String</span><span class="sxs-lookup"><span data-stu-id="8d7bc-177">String</span></span>|<span data-ttu-id="8d7bc-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-178">The developer of the app.</span></span> <span data-ttu-id="8d7bc-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-180">notes</span><span class="sxs-lookup"><span data-stu-id="8d7bc-180">notes</span></span>|<span data-ttu-id="8d7bc-181">String</span><span class="sxs-lookup"><span data-stu-id="8d7bc-181">String</span></span>|<span data-ttu-id="8d7bc-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-182">Notes for the app.</span></span> <span data-ttu-id="8d7bc-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8d7bc-184">uploadState</span></span>|<span data-ttu-id="8d7bc-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8d7bc-185">Int32</span></span>|<span data-ttu-id="8d7bc-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-186">The upload state.</span></span> <span data-ttu-id="8d7bc-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="8d7bc-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="8d7bc-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="8d7bc-189">publishingState</span></span>|[<span data-ttu-id="8d7bc-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8d7bc-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8d7bc-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-191">The publishing state for the app.</span></span> <span data-ttu-id="8d7bc-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8d7bc-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d7bc-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8d7bc-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8d7bc-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8d7bc-195">isAssigned</span></span>|<span data-ttu-id="8d7bc-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d7bc-196">Boolean</span></span>|<span data-ttu-id="8d7bc-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8d7bc-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d7bc-199">roleScopeTagIds</span></span>|<span data-ttu-id="8d7bc-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d7bc-200">String collection</span></span>|<span data-ttu-id="8d7bc-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8d7bc-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8d7bc-203">dependentAppCount</span></span>|<span data-ttu-id="8d7bc-204">Int32</span><span class="sxs-lookup"><span data-stu-id="8d7bc-204">Int32</span></span>|<span data-ttu-id="8d7bc-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8d7bc-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="8d7bc-207">supersedingAppCount</span></span>|<span data-ttu-id="8d7bc-208">Int32</span><span class="sxs-lookup"><span data-stu-id="8d7bc-208">Int32</span></span>|<span data-ttu-id="8d7bc-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="8d7bc-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="8d7bc-211">supersededAppCount</span></span>|<span data-ttu-id="8d7bc-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8d7bc-212">Int32</span></span>|<span data-ttu-id="8d7bc-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="8d7bc-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d7bc-215">packageId</span><span class="sxs-lookup"><span data-stu-id="8d7bc-215">packageId</span></span>|<span data-ttu-id="8d7bc-216">String</span><span class="sxs-lookup"><span data-stu-id="8d7bc-216">String</span></span>|<span data-ttu-id="8d7bc-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-217">The package identifier.</span></span>|
|<span data-ttu-id="8d7bc-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8d7bc-218">appIdentifier</span></span>|<span data-ttu-id="8d7bc-219">String</span><span class="sxs-lookup"><span data-stu-id="8d7bc-219">String</span></span>|<span data-ttu-id="8d7bc-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-220">The Identity Name.</span></span>|
|<span data-ttu-id="8d7bc-221">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8d7bc-221">usedLicenseCount</span></span>|<span data-ttu-id="8d7bc-222">Int32</span><span class="sxs-lookup"><span data-stu-id="8d7bc-222">Int32</span></span>|<span data-ttu-id="8d7bc-223">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-223">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="8d7bc-224">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8d7bc-224">totalLicenseCount</span></span>|<span data-ttu-id="8d7bc-225">Int32</span><span class="sxs-lookup"><span data-stu-id="8d7bc-225">Int32</span></span>|<span data-ttu-id="8d7bc-226">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-226">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="8d7bc-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8d7bc-227">appStoreUrl</span></span>|<span data-ttu-id="8d7bc-228">String</span><span class="sxs-lookup"><span data-stu-id="8d7bc-228">String</span></span>|<span data-ttu-id="8d7bc-229">A URL do aplicativo Play for Work Store.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-229">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="8d7bc-230">isPrivate</span><span class="sxs-lookup"><span data-stu-id="8d7bc-230">isPrivate</span></span>|<span data-ttu-id="8d7bc-231">Booleano</span><span class="sxs-lookup"><span data-stu-id="8d7bc-231">Boolean</span></span>|<span data-ttu-id="8d7bc-232">Indica se o aplicativo só está disponível para usuários de uma determinada empresa.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-232">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="8d7bc-233">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="8d7bc-233">isSystemApp</span></span>|<span data-ttu-id="8d7bc-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="8d7bc-234">Boolean</span></span>|<span data-ttu-id="8d7bc-235">Indica se o aplicativo é um aplicativo do sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-235">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="8d7bc-236">appTracks</span><span class="sxs-lookup"><span data-stu-id="8d7bc-236">appTracks</span></span>|<span data-ttu-id="8d7bc-237">[Coleção androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="8d7bc-237">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="8d7bc-238">As faixas que estão visíveis para essa empresa.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-238">The tracks that are visible to this enterprise.</span></span>|
|<span data-ttu-id="8d7bc-239">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="8d7bc-239">supportsOemConfig</span></span>|<span data-ttu-id="8d7bc-240">Booleano</span><span class="sxs-lookup"><span data-stu-id="8d7bc-240">Boolean</span></span>|<span data-ttu-id="8d7bc-241">Se esse aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-241">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8d7bc-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d7bc-242">Response</span></span>
<span data-ttu-id="8d7bc-243">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-243">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d7bc-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d7bc-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d7bc-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d7bc-245">Request</span></span>
<span data-ttu-id="8d7bc-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1225

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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

### <a name="response"></a><span data-ttu-id="8d7bc-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d7bc-247">Response</span></span>
<span data-ttu-id="8d7bc-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d7bc-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1397

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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




