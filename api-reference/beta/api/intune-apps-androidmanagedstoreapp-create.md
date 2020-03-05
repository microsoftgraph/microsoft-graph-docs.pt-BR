---
title: Criar androidManagedStoreApp
description: Criar um novo objeto androidManagedStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 758456e0e02780ce3cf839df75953abee72bf8e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445943"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="29105-103">Criar androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="29105-103">Create androidManagedStoreApp</span></span>

<span data-ttu-id="29105-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29105-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29105-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29105-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29105-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29105-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29105-107">Criar um novo objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="29105-107">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29105-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29105-108">Prerequisites</span></span>
<span data-ttu-id="29105-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29105-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29105-111">Permission type</span></span>|<span data-ttu-id="29105-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29105-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29105-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29105-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29105-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29105-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="29105-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29105-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29105-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29105-116">Not supported.</span></span>|
|<span data-ttu-id="29105-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29105-117">Application</span></span>|<span data-ttu-id="29105-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29105-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29105-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29105-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="29105-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29105-120">Request headers</span></span>
|<span data-ttu-id="29105-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29105-121">Header</span></span>|<span data-ttu-id="29105-122">Valor</span><span class="sxs-lookup"><span data-stu-id="29105-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29105-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29105-123">Authorization</span></span>|<span data-ttu-id="29105-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29105-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29105-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29105-125">Accept</span></span>|<span data-ttu-id="29105-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29105-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29105-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29105-127">Request body</span></span>
<span data-ttu-id="29105-128">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="29105-128">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="29105-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="29105-129">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="29105-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29105-130">Property</span></span>|<span data-ttu-id="29105-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="29105-131">Type</span></span>|<span data-ttu-id="29105-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="29105-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29105-133">id</span><span class="sxs-lookup"><span data-stu-id="29105-133">id</span></span>|<span data-ttu-id="29105-134">String</span><span class="sxs-lookup"><span data-stu-id="29105-134">String</span></span>|<span data-ttu-id="29105-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="29105-135">Key of the entity.</span></span> <span data-ttu-id="29105-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-137">displayName</span><span class="sxs-lookup"><span data-stu-id="29105-137">displayName</span></span>|<span data-ttu-id="29105-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29105-138">String</span></span>|<span data-ttu-id="29105-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="29105-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="29105-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-141">description</span><span class="sxs-lookup"><span data-stu-id="29105-141">description</span></span>|<span data-ttu-id="29105-142">String</span><span class="sxs-lookup"><span data-stu-id="29105-142">String</span></span>|<span data-ttu-id="29105-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29105-143">The description of the app.</span></span> <span data-ttu-id="29105-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-145">publicador</span><span class="sxs-lookup"><span data-stu-id="29105-145">publisher</span></span>|<span data-ttu-id="29105-146">String</span><span class="sxs-lookup"><span data-stu-id="29105-146">String</span></span>|<span data-ttu-id="29105-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29105-147">The publisher of the app.</span></span> <span data-ttu-id="29105-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="29105-149">largeIcon</span></span>|[<span data-ttu-id="29105-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="29105-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="29105-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="29105-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="29105-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29105-153">createdDateTime</span></span>|<span data-ttu-id="29105-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29105-154">DateTimeOffset</span></span>|<span data-ttu-id="29105-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29105-155">The date and time the app was created.</span></span> <span data-ttu-id="29105-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29105-157">lastModifiedDateTime</span></span>|<span data-ttu-id="29105-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29105-158">DateTimeOffset</span></span>|<span data-ttu-id="29105-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="29105-159">The date and time the app was last modified.</span></span> <span data-ttu-id="29105-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="29105-161">isFeatured</span></span>|<span data-ttu-id="29105-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="29105-162">Boolean</span></span>|<span data-ttu-id="29105-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="29105-164">privacyInformationUrl</span></span>|<span data-ttu-id="29105-165">String</span><span class="sxs-lookup"><span data-stu-id="29105-165">String</span></span>|<span data-ttu-id="29105-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="29105-166">The privacy statement Url.</span></span> <span data-ttu-id="29105-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="29105-168">informationUrl</span></span>|<span data-ttu-id="29105-169">String</span><span class="sxs-lookup"><span data-stu-id="29105-169">String</span></span>|<span data-ttu-id="29105-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="29105-170">The more information Url.</span></span> <span data-ttu-id="29105-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-172">owner</span><span class="sxs-lookup"><span data-stu-id="29105-172">owner</span></span>|<span data-ttu-id="29105-173">String</span><span class="sxs-lookup"><span data-stu-id="29105-173">String</span></span>|<span data-ttu-id="29105-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="29105-174">The owner of the app.</span></span> <span data-ttu-id="29105-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-176">developer</span><span class="sxs-lookup"><span data-stu-id="29105-176">developer</span></span>|<span data-ttu-id="29105-177">String</span><span class="sxs-lookup"><span data-stu-id="29105-177">String</span></span>|<span data-ttu-id="29105-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29105-178">The developer of the app.</span></span> <span data-ttu-id="29105-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-180">notes</span><span class="sxs-lookup"><span data-stu-id="29105-180">notes</span></span>|<span data-ttu-id="29105-181">String</span><span class="sxs-lookup"><span data-stu-id="29105-181">String</span></span>|<span data-ttu-id="29105-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29105-182">Notes for the app.</span></span> <span data-ttu-id="29105-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="29105-184">uploadState</span></span>|<span data-ttu-id="29105-185">Int32</span><span class="sxs-lookup"><span data-stu-id="29105-185">Int32</span></span>|<span data-ttu-id="29105-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="29105-186">The upload state.</span></span> <span data-ttu-id="29105-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="29105-188">publishingState</span></span>|[<span data-ttu-id="29105-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="29105-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="29105-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29105-190">The publishing state for the app.</span></span> <span data-ttu-id="29105-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="29105-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="29105-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29105-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="29105-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="29105-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="29105-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="29105-194">isAssigned</span></span>|<span data-ttu-id="29105-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="29105-195">Boolean</span></span>|<span data-ttu-id="29105-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="29105-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="29105-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="29105-198">roleScopeTagIds</span></span>|<span data-ttu-id="29105-199">String collection</span><span class="sxs-lookup"><span data-stu-id="29105-199">String collection</span></span>|<span data-ttu-id="29105-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="29105-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="29105-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="29105-202">dependentAppCount</span></span>|<span data-ttu-id="29105-203">Int32</span><span class="sxs-lookup"><span data-stu-id="29105-203">Int32</span></span>|<span data-ttu-id="29105-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="29105-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="29105-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29105-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="29105-206">packageId</span><span class="sxs-lookup"><span data-stu-id="29105-206">packageId</span></span>|<span data-ttu-id="29105-207">String</span><span class="sxs-lookup"><span data-stu-id="29105-207">String</span></span>|<span data-ttu-id="29105-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="29105-208">The package identifier.</span></span>|
|<span data-ttu-id="29105-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="29105-209">appIdentifier</span></span>|<span data-ttu-id="29105-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29105-210">String</span></span>|<span data-ttu-id="29105-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="29105-211">The Identity Name.</span></span>|
|<span data-ttu-id="29105-212">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="29105-212">usedLicenseCount</span></span>|<span data-ttu-id="29105-213">Int32</span><span class="sxs-lookup"><span data-stu-id="29105-213">Int32</span></span>|<span data-ttu-id="29105-214">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="29105-214">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="29105-215">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="29105-215">totalLicenseCount</span></span>|<span data-ttu-id="29105-216">Int32</span><span class="sxs-lookup"><span data-stu-id="29105-216">Int32</span></span>|<span data-ttu-id="29105-217">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="29105-217">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="29105-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="29105-218">appStoreUrl</span></span>|<span data-ttu-id="29105-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29105-219">String</span></span>|<span data-ttu-id="29105-220">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="29105-220">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="29105-221">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="29105-221">isPrivate</span></span>|<span data-ttu-id="29105-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="29105-222">Boolean</span></span>|<span data-ttu-id="29105-223">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="29105-223">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="29105-224">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="29105-224">isSystemApp</span></span>|<span data-ttu-id="29105-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="29105-225">Boolean</span></span>|<span data-ttu-id="29105-226">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="29105-226">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="29105-227">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="29105-227">supportsOemConfig</span></span>|<span data-ttu-id="29105-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="29105-228">Boolean</span></span>|<span data-ttu-id="29105-229">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="29105-229">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="29105-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="29105-230">Response</span></span>
<span data-ttu-id="29105-231">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29105-231">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29105-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29105-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="29105-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29105-233">Request</span></span>
<span data-ttu-id="29105-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29105-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 984

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="29105-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="29105-235">Response</span></span>
<span data-ttu-id="29105-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29105-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1156

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```





