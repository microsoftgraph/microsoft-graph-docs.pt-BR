---
title: Criar androidManagedStoreWebApp
description: Criar um novo objeto androidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c921b5260783a59d2ed3803de5a6235abf61287
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790095"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="6cb67-103">Criar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="6cb67-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="6cb67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cb67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cb67-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6cb67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cb67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cb67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cb67-107">Criar um novo objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="6cb67-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cb67-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cb67-108">Prerequisites</span></span>
<span data-ttu-id="6cb67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb67-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cb67-111">Permission type</span></span>|<span data-ttu-id="6cb67-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cb67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cb67-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cb67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cb67-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb67-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6cb67-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cb67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cb67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cb67-116">Not supported.</span></span>|
|<span data-ttu-id="6cb67-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cb67-117">Application</span></span>|<span data-ttu-id="6cb67-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb67-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cb67-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6cb67-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb67-120">Request headers</span></span>
|<span data-ttu-id="6cb67-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cb67-121">Header</span></span>|<span data-ttu-id="6cb67-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6cb67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cb67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cb67-123">Authorization</span></span>|<span data-ttu-id="6cb67-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cb67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cb67-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cb67-125">Accept</span></span>|<span data-ttu-id="6cb67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cb67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cb67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb67-127">Request body</span></span>
<span data-ttu-id="6cb67-128">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="6cb67-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="6cb67-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="6cb67-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="6cb67-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cb67-130">Property</span></span>|<span data-ttu-id="6cb67-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cb67-131">Type</span></span>|<span data-ttu-id="6cb67-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cb67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cb67-133">id</span><span class="sxs-lookup"><span data-stu-id="6cb67-133">id</span></span>|<span data-ttu-id="6cb67-134">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-134">String</span></span>|<span data-ttu-id="6cb67-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6cb67-135">Key of the entity.</span></span> <span data-ttu-id="6cb67-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6cb67-137">displayName</span></span>|<span data-ttu-id="6cb67-138">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-138">String</span></span>|<span data-ttu-id="6cb67-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6cb67-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6cb67-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-141">description</span><span class="sxs-lookup"><span data-stu-id="6cb67-141">description</span></span>|<span data-ttu-id="6cb67-142">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-142">String</span></span>|<span data-ttu-id="6cb67-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb67-143">The description of the app.</span></span> <span data-ttu-id="6cb67-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-145">publicador</span><span class="sxs-lookup"><span data-stu-id="6cb67-145">publisher</span></span>|<span data-ttu-id="6cb67-146">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-146">String</span></span>|<span data-ttu-id="6cb67-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb67-147">The publisher of the app.</span></span> <span data-ttu-id="6cb67-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6cb67-149">largeIcon</span></span>|[<span data-ttu-id="6cb67-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6cb67-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6cb67-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6cb67-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6cb67-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cb67-153">createdDateTime</span></span>|<span data-ttu-id="6cb67-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cb67-154">DateTimeOffset</span></span>|<span data-ttu-id="6cb67-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb67-155">The date and time the app was created.</span></span> <span data-ttu-id="6cb67-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cb67-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6cb67-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cb67-158">DateTimeOffset</span></span>|<span data-ttu-id="6cb67-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6cb67-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6cb67-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6cb67-161">isFeatured</span></span>|<span data-ttu-id="6cb67-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cb67-162">Boolean</span></span>|<span data-ttu-id="6cb67-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6cb67-164">privacyInformationUrl</span></span>|<span data-ttu-id="6cb67-165">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-165">String</span></span>|<span data-ttu-id="6cb67-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6cb67-166">The privacy statement Url.</span></span> <span data-ttu-id="6cb67-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6cb67-168">informationUrl</span></span>|<span data-ttu-id="6cb67-169">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-169">String</span></span>|<span data-ttu-id="6cb67-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6cb67-170">The more information Url.</span></span> <span data-ttu-id="6cb67-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-172">owner</span><span class="sxs-lookup"><span data-stu-id="6cb67-172">owner</span></span>|<span data-ttu-id="6cb67-173">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-173">String</span></span>|<span data-ttu-id="6cb67-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6cb67-174">The owner of the app.</span></span> <span data-ttu-id="6cb67-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-176">developer</span><span class="sxs-lookup"><span data-stu-id="6cb67-176">developer</span></span>|<span data-ttu-id="6cb67-177">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-177">String</span></span>|<span data-ttu-id="6cb67-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb67-178">The developer of the app.</span></span> <span data-ttu-id="6cb67-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-180">notes</span><span class="sxs-lookup"><span data-stu-id="6cb67-180">notes</span></span>|<span data-ttu-id="6cb67-181">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-181">String</span></span>|<span data-ttu-id="6cb67-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb67-182">Notes for the app.</span></span> <span data-ttu-id="6cb67-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6cb67-184">uploadState</span></span>|<span data-ttu-id="6cb67-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6cb67-185">Int32</span></span>|<span data-ttu-id="6cb67-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="6cb67-186">The upload state.</span></span> <span data-ttu-id="6cb67-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="6cb67-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="6cb67-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="6cb67-189">publishingState</span></span>|[<span data-ttu-id="6cb67-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6cb67-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6cb67-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb67-191">The publishing state for the app.</span></span> <span data-ttu-id="6cb67-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6cb67-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6cb67-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cb67-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6cb67-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6cb67-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6cb67-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6cb67-195">isAssigned</span></span>|<span data-ttu-id="6cb67-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cb67-196">Boolean</span></span>|<span data-ttu-id="6cb67-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="6cb67-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6cb67-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6cb67-199">roleScopeTagIds</span></span>|<span data-ttu-id="6cb67-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cb67-200">String collection</span></span>|<span data-ttu-id="6cb67-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6cb67-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6cb67-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6cb67-203">dependentAppCount</span></span>|<span data-ttu-id="6cb67-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6cb67-204">Int32</span></span>|<span data-ttu-id="6cb67-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="6cb67-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6cb67-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cb67-207">packageId</span><span class="sxs-lookup"><span data-stu-id="6cb67-207">packageId</span></span>|<span data-ttu-id="6cb67-208">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-208">String</span></span>|<span data-ttu-id="6cb67-209">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="6cb67-209">The package identifier.</span></span> <span data-ttu-id="6cb67-210">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-210">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6cb67-211">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6cb67-211">appIdentifier</span></span>|<span data-ttu-id="6cb67-212">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-212">String</span></span>|<span data-ttu-id="6cb67-213">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6cb67-213">The Identity Name.</span></span> <span data-ttu-id="6cb67-214">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-214">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6cb67-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6cb67-215">usedLicenseCount</span></span>|<span data-ttu-id="6cb67-216">Int32</span><span class="sxs-lookup"><span data-stu-id="6cb67-216">Int32</span></span>|<span data-ttu-id="6cb67-217">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="6cb67-217">The number of VPP licenses in use.</span></span> <span data-ttu-id="6cb67-218">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6cb67-219">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6cb67-219">totalLicenseCount</span></span>|<span data-ttu-id="6cb67-220">Int32</span><span class="sxs-lookup"><span data-stu-id="6cb67-220">Int32</span></span>|<span data-ttu-id="6cb67-221">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="6cb67-221">The total number of VPP licenses.</span></span> <span data-ttu-id="6cb67-222">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6cb67-223">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6cb67-223">appStoreUrl</span></span>|<span data-ttu-id="6cb67-224">String</span><span class="sxs-lookup"><span data-stu-id="6cb67-224">String</span></span>|<span data-ttu-id="6cb67-225">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6cb67-225">The Play for Work Store app URL.</span></span> <span data-ttu-id="6cb67-226">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6cb67-227">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="6cb67-227">isPrivate</span></span>|<span data-ttu-id="6cb67-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cb67-228">Boolean</span></span>|<span data-ttu-id="6cb67-229">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="6cb67-229">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="6cb67-230">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6cb67-231">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="6cb67-231">isSystemApp</span></span>|<span data-ttu-id="6cb67-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cb67-232">Boolean</span></span>|<span data-ttu-id="6cb67-233">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="6cb67-233">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="6cb67-234">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6cb67-235">appTracks</span><span class="sxs-lookup"><span data-stu-id="6cb67-235">appTracks</span></span>|<span data-ttu-id="6cb67-236">coleção [androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-236">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="6cb67-237">As faixas que são visíveis para esta empresa.</span><span class="sxs-lookup"><span data-stu-id="6cb67-237">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="6cb67-238">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="6cb67-239">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="6cb67-239">supportsOemConfig</span></span>|<span data-ttu-id="6cb67-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cb67-240">Boolean</span></span>|<span data-ttu-id="6cb67-241">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="6cb67-241">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="6cb67-242">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cb67-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6cb67-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb67-243">Response</span></span>
<span data-ttu-id="6cb67-244">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cb67-244">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cb67-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cb67-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cb67-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb67-246">Request</span></span>
<span data-ttu-id="6cb67-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cb67-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="6cb67-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb67-248">Response</span></span>
<span data-ttu-id="6cb67-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cb67-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



