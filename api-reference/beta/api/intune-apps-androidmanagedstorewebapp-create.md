---
title: Criar androidManagedStoreWebApp
description: Criar um novo objeto androidManagedStoreWebApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ba24aabb3d53979d34e20da80d462156939d154
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535489"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="02800-103">Criar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="02800-103">Create androidManagedStoreWebApp</span></span>

> <span data-ttu-id="02800-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02800-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02800-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02800-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02800-106">Criar um novo objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="02800-106">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02800-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02800-107">Prerequisites</span></span>
<span data-ttu-id="02800-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02800-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02800-110">Permission type</span></span>|<span data-ttu-id="02800-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02800-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02800-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02800-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02800-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02800-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02800-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02800-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02800-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02800-115">Not supported.</span></span>|
|<span data-ttu-id="02800-116">Application</span><span class="sxs-lookup"><span data-stu-id="02800-116">Application</span></span>|<span data-ttu-id="02800-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02800-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02800-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02800-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="02800-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02800-119">Request headers</span></span>
|<span data-ttu-id="02800-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02800-120">Header</span></span>|<span data-ttu-id="02800-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02800-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02800-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02800-122">Authorization</span></span>|<span data-ttu-id="02800-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02800-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02800-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02800-124">Accept</span></span>|<span data-ttu-id="02800-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02800-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02800-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02800-126">Request body</span></span>
<span data-ttu-id="02800-127">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="02800-127">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="02800-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="02800-128">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="02800-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02800-129">Property</span></span>|<span data-ttu-id="02800-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="02800-130">Type</span></span>|<span data-ttu-id="02800-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="02800-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02800-132">id</span><span class="sxs-lookup"><span data-stu-id="02800-132">id</span></span>|<span data-ttu-id="02800-133">String</span><span class="sxs-lookup"><span data-stu-id="02800-133">String</span></span>|<span data-ttu-id="02800-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02800-134">Key of the entity.</span></span> <span data-ttu-id="02800-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-136">displayName</span><span class="sxs-lookup"><span data-stu-id="02800-136">displayName</span></span>|<span data-ttu-id="02800-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-137">String</span></span>|<span data-ttu-id="02800-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="02800-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="02800-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-140">description</span><span class="sxs-lookup"><span data-stu-id="02800-140">description</span></span>|<span data-ttu-id="02800-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-141">String</span></span>|<span data-ttu-id="02800-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02800-142">The description of the app.</span></span> <span data-ttu-id="02800-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-144">publicador</span><span class="sxs-lookup"><span data-stu-id="02800-144">publisher</span></span>|<span data-ttu-id="02800-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-145">String</span></span>|<span data-ttu-id="02800-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02800-146">The publisher of the app.</span></span> <span data-ttu-id="02800-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="02800-148">largeIcon</span></span>|[<span data-ttu-id="02800-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="02800-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="02800-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="02800-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="02800-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02800-152">createdDateTime</span></span>|<span data-ttu-id="02800-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02800-153">DateTimeOffset</span></span>|<span data-ttu-id="02800-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02800-154">The date and time the app was created.</span></span> <span data-ttu-id="02800-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02800-156">lastModifiedDateTime</span></span>|<span data-ttu-id="02800-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02800-157">DateTimeOffset</span></span>|<span data-ttu-id="02800-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="02800-158">The date and time the app was last modified.</span></span> <span data-ttu-id="02800-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="02800-160">isFeatured</span></span>|<span data-ttu-id="02800-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="02800-161">Boolean</span></span>|<span data-ttu-id="02800-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="02800-163">privacyInformationUrl</span></span>|<span data-ttu-id="02800-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-164">String</span></span>|<span data-ttu-id="02800-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="02800-165">The privacy statement Url.</span></span> <span data-ttu-id="02800-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="02800-167">informationUrl</span></span>|<span data-ttu-id="02800-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-168">String</span></span>|<span data-ttu-id="02800-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="02800-169">The more information Url.</span></span> <span data-ttu-id="02800-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-171">owner</span><span class="sxs-lookup"><span data-stu-id="02800-171">owner</span></span>|<span data-ttu-id="02800-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-172">String</span></span>|<span data-ttu-id="02800-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="02800-173">The owner of the app.</span></span> <span data-ttu-id="02800-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-175">developer</span><span class="sxs-lookup"><span data-stu-id="02800-175">developer</span></span>|<span data-ttu-id="02800-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-176">String</span></span>|<span data-ttu-id="02800-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02800-177">The developer of the app.</span></span> <span data-ttu-id="02800-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-179">notes</span><span class="sxs-lookup"><span data-stu-id="02800-179">notes</span></span>|<span data-ttu-id="02800-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-180">String</span></span>|<span data-ttu-id="02800-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02800-181">Notes for the app.</span></span> <span data-ttu-id="02800-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="02800-183">uploadState</span></span>|<span data-ttu-id="02800-184">Int32</span><span class="sxs-lookup"><span data-stu-id="02800-184">Int32</span></span>|<span data-ttu-id="02800-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="02800-185">The upload state.</span></span> <span data-ttu-id="02800-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="02800-187">publishingState</span></span>|[<span data-ttu-id="02800-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="02800-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="02800-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02800-189">The publishing state for the app.</span></span> <span data-ttu-id="02800-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="02800-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="02800-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02800-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="02800-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="02800-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="02800-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="02800-193">isAssigned</span></span>|<span data-ttu-id="02800-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="02800-194">Boolean</span></span>|<span data-ttu-id="02800-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="02800-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="02800-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="02800-197">roleScopeTagIds</span></span>|<span data-ttu-id="02800-198">String collection</span><span class="sxs-lookup"><span data-stu-id="02800-198">String collection</span></span>|<span data-ttu-id="02800-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="02800-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="02800-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="02800-201">dependentAppCount</span></span>|<span data-ttu-id="02800-202">Int32</span><span class="sxs-lookup"><span data-stu-id="02800-202">Int32</span></span>|<span data-ttu-id="02800-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="02800-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="02800-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02800-205">packageId</span><span class="sxs-lookup"><span data-stu-id="02800-205">packageId</span></span>|<span data-ttu-id="02800-206">String</span><span class="sxs-lookup"><span data-stu-id="02800-206">String</span></span>|<span data-ttu-id="02800-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="02800-207">The package identifier.</span></span> <span data-ttu-id="02800-208">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-208">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="02800-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="02800-209">appIdentifier</span></span>|<span data-ttu-id="02800-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-210">String</span></span>|<span data-ttu-id="02800-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="02800-211">The Identity Name.</span></span> <span data-ttu-id="02800-212">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-212">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="02800-213">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="02800-213">usedLicenseCount</span></span>|<span data-ttu-id="02800-214">Int32</span><span class="sxs-lookup"><span data-stu-id="02800-214">Int32</span></span>|<span data-ttu-id="02800-215">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="02800-215">The number of VPP licenses in use.</span></span> <span data-ttu-id="02800-216">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-216">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="02800-217">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="02800-217">totalLicenseCount</span></span>|<span data-ttu-id="02800-218">Int32</span><span class="sxs-lookup"><span data-stu-id="02800-218">Int32</span></span>|<span data-ttu-id="02800-219">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="02800-219">The total number of VPP licenses.</span></span> <span data-ttu-id="02800-220">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-220">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="02800-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="02800-221">appStoreUrl</span></span>|<span data-ttu-id="02800-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02800-222">String</span></span>|<span data-ttu-id="02800-223">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="02800-223">The Play for Work Store app URL.</span></span> <span data-ttu-id="02800-224">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-224">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="02800-225">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="02800-225">isPrivate</span></span>|<span data-ttu-id="02800-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="02800-226">Boolean</span></span>|<span data-ttu-id="02800-227">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="02800-227">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="02800-228">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-228">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="02800-229">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="02800-229">isSystemApp</span></span>|<span data-ttu-id="02800-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="02800-230">Boolean</span></span>|<span data-ttu-id="02800-231">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="02800-231">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="02800-232">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-232">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="02800-233">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="02800-233">supportsOemConfig</span></span>|<span data-ttu-id="02800-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="02800-234">Boolean</span></span>|<span data-ttu-id="02800-235">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="02800-235">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="02800-236">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="02800-236">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="02800-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="02800-237">Response</span></span>
<span data-ttu-id="02800-238">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02800-238">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02800-239">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02800-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="02800-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02800-240">Request</span></span>
<span data-ttu-id="02800-241">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02800-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 987

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
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="02800-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="02800-242">Response</span></span>
<span data-ttu-id="02800-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02800-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1159

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
  "supportsOemConfig": true
}
```






