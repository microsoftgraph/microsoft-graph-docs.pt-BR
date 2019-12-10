---
title: Criar androidManagedStoreApp
description: Criar um novo objeto androidManagedStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5d1cfa1d0c8abb1cdae737539eaa827afc25504
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39926674"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="30ee7-103">Criar androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="30ee7-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="30ee7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30ee7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30ee7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30ee7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30ee7-106">Criar um novo objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="30ee7-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30ee7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30ee7-107">Prerequisites</span></span>
<span data-ttu-id="30ee7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30ee7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30ee7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30ee7-110">Permission type</span></span>|<span data-ttu-id="30ee7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30ee7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30ee7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30ee7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30ee7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30ee7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30ee7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30ee7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30ee7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30ee7-115">Not supported.</span></span>|
|<span data-ttu-id="30ee7-116">Application</span><span class="sxs-lookup"><span data-stu-id="30ee7-116">Application</span></span>|<span data-ttu-id="30ee7-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30ee7-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30ee7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30ee7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="30ee7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30ee7-119">Request headers</span></span>
|<span data-ttu-id="30ee7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30ee7-120">Header</span></span>|<span data-ttu-id="30ee7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="30ee7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30ee7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="30ee7-122">Authorization</span></span>|<span data-ttu-id="30ee7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30ee7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30ee7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30ee7-124">Accept</span></span>|<span data-ttu-id="30ee7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30ee7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30ee7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30ee7-126">Request body</span></span>
<span data-ttu-id="30ee7-127">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="30ee7-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="30ee7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="30ee7-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="30ee7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30ee7-129">Property</span></span>|<span data-ttu-id="30ee7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="30ee7-130">Type</span></span>|<span data-ttu-id="30ee7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="30ee7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30ee7-132">id</span><span class="sxs-lookup"><span data-stu-id="30ee7-132">id</span></span>|<span data-ttu-id="30ee7-133">String</span><span class="sxs-lookup"><span data-stu-id="30ee7-133">String</span></span>|<span data-ttu-id="30ee7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="30ee7-134">Key of the entity.</span></span> <span data-ttu-id="30ee7-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="30ee7-136">displayName</span></span>|<span data-ttu-id="30ee7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-137">String</span></span>|<span data-ttu-id="30ee7-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="30ee7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="30ee7-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-140">description</span><span class="sxs-lookup"><span data-stu-id="30ee7-140">description</span></span>|<span data-ttu-id="30ee7-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-141">String</span></span>|<span data-ttu-id="30ee7-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30ee7-142">The description of the app.</span></span> <span data-ttu-id="30ee7-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-144">publicador</span><span class="sxs-lookup"><span data-stu-id="30ee7-144">publisher</span></span>|<span data-ttu-id="30ee7-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-145">String</span></span>|<span data-ttu-id="30ee7-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30ee7-146">The publisher of the app.</span></span> <span data-ttu-id="30ee7-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="30ee7-148">largeIcon</span></span>|[<span data-ttu-id="30ee7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="30ee7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="30ee7-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="30ee7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="30ee7-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30ee7-152">createdDateTime</span></span>|<span data-ttu-id="30ee7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30ee7-153">DateTimeOffset</span></span>|<span data-ttu-id="30ee7-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30ee7-154">The date and time the app was created.</span></span> <span data-ttu-id="30ee7-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30ee7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="30ee7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30ee7-157">DateTimeOffset</span></span>|<span data-ttu-id="30ee7-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="30ee7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="30ee7-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="30ee7-160">isFeatured</span></span>|<span data-ttu-id="30ee7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="30ee7-161">Boolean</span></span>|<span data-ttu-id="30ee7-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="30ee7-163">privacyInformationUrl</span></span>|<span data-ttu-id="30ee7-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-164">String</span></span>|<span data-ttu-id="30ee7-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="30ee7-165">The privacy statement Url.</span></span> <span data-ttu-id="30ee7-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="30ee7-167">informationUrl</span></span>|<span data-ttu-id="30ee7-168">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-168">String</span></span>|<span data-ttu-id="30ee7-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="30ee7-169">The more information Url.</span></span> <span data-ttu-id="30ee7-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-171">owner</span><span class="sxs-lookup"><span data-stu-id="30ee7-171">owner</span></span>|<span data-ttu-id="30ee7-172">String</span><span class="sxs-lookup"><span data-stu-id="30ee7-172">String</span></span>|<span data-ttu-id="30ee7-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="30ee7-173">The owner of the app.</span></span> <span data-ttu-id="30ee7-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-175">developer</span><span class="sxs-lookup"><span data-stu-id="30ee7-175">developer</span></span>|<span data-ttu-id="30ee7-176">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-176">String</span></span>|<span data-ttu-id="30ee7-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30ee7-177">The developer of the app.</span></span> <span data-ttu-id="30ee7-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-179">notes</span><span class="sxs-lookup"><span data-stu-id="30ee7-179">notes</span></span>|<span data-ttu-id="30ee7-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-180">String</span></span>|<span data-ttu-id="30ee7-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30ee7-181">Notes for the app.</span></span> <span data-ttu-id="30ee7-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="30ee7-183">uploadState</span></span>|<span data-ttu-id="30ee7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="30ee7-184">Int32</span></span>|<span data-ttu-id="30ee7-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="30ee7-185">The upload state.</span></span> <span data-ttu-id="30ee7-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="30ee7-187">publishingState</span></span>|[<span data-ttu-id="30ee7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="30ee7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="30ee7-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30ee7-189">The publishing state for the app.</span></span> <span data-ttu-id="30ee7-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="30ee7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="30ee7-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30ee7-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="30ee7-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="30ee7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="30ee7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="30ee7-193">isAssigned</span></span>|<span data-ttu-id="30ee7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="30ee7-194">Boolean</span></span>|<span data-ttu-id="30ee7-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="30ee7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="30ee7-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30ee7-197">roleScopeTagIds</span></span>|<span data-ttu-id="30ee7-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-198">String collection</span></span>|<span data-ttu-id="30ee7-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="30ee7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="30ee7-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="30ee7-201">dependentAppCount</span></span>|<span data-ttu-id="30ee7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="30ee7-202">Int32</span></span>|<span data-ttu-id="30ee7-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="30ee7-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="30ee7-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30ee7-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30ee7-205">packageId</span><span class="sxs-lookup"><span data-stu-id="30ee7-205">packageId</span></span>|<span data-ttu-id="30ee7-206">String</span><span class="sxs-lookup"><span data-stu-id="30ee7-206">String</span></span>|<span data-ttu-id="30ee7-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="30ee7-207">The package identifier.</span></span>|
|<span data-ttu-id="30ee7-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="30ee7-208">appIdentifier</span></span>|<span data-ttu-id="30ee7-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-209">String</span></span>|<span data-ttu-id="30ee7-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="30ee7-210">The Identity Name.</span></span>|
|<span data-ttu-id="30ee7-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="30ee7-211">usedLicenseCount</span></span>|<span data-ttu-id="30ee7-212">Int32</span><span class="sxs-lookup"><span data-stu-id="30ee7-212">Int32</span></span>|<span data-ttu-id="30ee7-213">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="30ee7-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="30ee7-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="30ee7-214">totalLicenseCount</span></span>|<span data-ttu-id="30ee7-215">Int32</span><span class="sxs-lookup"><span data-stu-id="30ee7-215">Int32</span></span>|<span data-ttu-id="30ee7-216">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="30ee7-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="30ee7-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="30ee7-217">appStoreUrl</span></span>|<span data-ttu-id="30ee7-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30ee7-218">String</span></span>|<span data-ttu-id="30ee7-219">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="30ee7-219">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="30ee7-220">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="30ee7-220">isPrivate</span></span>|<span data-ttu-id="30ee7-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="30ee7-221">Boolean</span></span>|<span data-ttu-id="30ee7-222">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="30ee7-222">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="30ee7-223">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="30ee7-223">isSystemApp</span></span>|<span data-ttu-id="30ee7-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="30ee7-224">Boolean</span></span>|<span data-ttu-id="30ee7-225">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="30ee7-225">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="30ee7-226">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="30ee7-226">supportsOemConfig</span></span>|<span data-ttu-id="30ee7-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="30ee7-227">Boolean</span></span>|<span data-ttu-id="30ee7-228">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="30ee7-228">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="30ee7-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="30ee7-229">Response</span></span>
<span data-ttu-id="30ee7-230">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30ee7-230">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30ee7-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30ee7-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="30ee7-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30ee7-232">Request</span></span>
<span data-ttu-id="30ee7-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30ee7-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30ee7-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="30ee7-234">Response</span></span>
<span data-ttu-id="30ee7-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30ee7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





