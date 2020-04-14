---
title: Criar androidManagedStoreWebApp
description: Criar um novo objeto androidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c23d0df9033aa0f92c09ef6664776a154b3cfa3e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417411"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="64548-103">Criar androidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="64548-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="64548-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64548-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64548-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64548-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64548-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64548-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64548-107">Criar um novo objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="64548-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64548-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64548-108">Prerequisites</span></span>
<span data-ttu-id="64548-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64548-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64548-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64548-111">Permission type</span></span>|<span data-ttu-id="64548-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64548-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64548-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64548-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64548-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64548-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64548-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64548-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64548-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64548-116">Not supported.</span></span>|
|<span data-ttu-id="64548-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64548-117">Application</span></span>|<span data-ttu-id="64548-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64548-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64548-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64548-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="64548-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64548-120">Request headers</span></span>
|<span data-ttu-id="64548-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64548-121">Header</span></span>|<span data-ttu-id="64548-122">Valor</span><span class="sxs-lookup"><span data-stu-id="64548-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64548-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64548-123">Authorization</span></span>|<span data-ttu-id="64548-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64548-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64548-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64548-125">Accept</span></span>|<span data-ttu-id="64548-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64548-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64548-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64548-127">Request body</span></span>
<span data-ttu-id="64548-128">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="64548-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="64548-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="64548-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="64548-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64548-130">Property</span></span>|<span data-ttu-id="64548-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="64548-131">Type</span></span>|<span data-ttu-id="64548-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="64548-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64548-133">id</span><span class="sxs-lookup"><span data-stu-id="64548-133">id</span></span>|<span data-ttu-id="64548-134">String</span><span class="sxs-lookup"><span data-stu-id="64548-134">String</span></span>|<span data-ttu-id="64548-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="64548-135">Key of the entity.</span></span> <span data-ttu-id="64548-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-137">displayName</span><span class="sxs-lookup"><span data-stu-id="64548-137">displayName</span></span>|<span data-ttu-id="64548-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64548-138">String</span></span>|<span data-ttu-id="64548-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="64548-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="64548-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-141">description</span><span class="sxs-lookup"><span data-stu-id="64548-141">description</span></span>|<span data-ttu-id="64548-142">String</span><span class="sxs-lookup"><span data-stu-id="64548-142">String</span></span>|<span data-ttu-id="64548-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64548-143">The description of the app.</span></span> <span data-ttu-id="64548-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-145">publicador</span><span class="sxs-lookup"><span data-stu-id="64548-145">publisher</span></span>|<span data-ttu-id="64548-146">String</span><span class="sxs-lookup"><span data-stu-id="64548-146">String</span></span>|<span data-ttu-id="64548-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64548-147">The publisher of the app.</span></span> <span data-ttu-id="64548-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="64548-149">largeIcon</span></span>|[<span data-ttu-id="64548-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="64548-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="64548-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="64548-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="64548-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64548-153">createdDateTime</span></span>|<span data-ttu-id="64548-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64548-154">DateTimeOffset</span></span>|<span data-ttu-id="64548-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64548-155">The date and time the app was created.</span></span> <span data-ttu-id="64548-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64548-157">lastModifiedDateTime</span></span>|<span data-ttu-id="64548-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64548-158">DateTimeOffset</span></span>|<span data-ttu-id="64548-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="64548-159">The date and time the app was last modified.</span></span> <span data-ttu-id="64548-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="64548-161">isFeatured</span></span>|<span data-ttu-id="64548-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="64548-162">Boolean</span></span>|<span data-ttu-id="64548-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="64548-164">privacyInformationUrl</span></span>|<span data-ttu-id="64548-165">String</span><span class="sxs-lookup"><span data-stu-id="64548-165">String</span></span>|<span data-ttu-id="64548-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="64548-166">The privacy statement Url.</span></span> <span data-ttu-id="64548-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="64548-168">informationUrl</span></span>|<span data-ttu-id="64548-169">String</span><span class="sxs-lookup"><span data-stu-id="64548-169">String</span></span>|<span data-ttu-id="64548-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="64548-170">The more information Url.</span></span> <span data-ttu-id="64548-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-172">owner</span><span class="sxs-lookup"><span data-stu-id="64548-172">owner</span></span>|<span data-ttu-id="64548-173">String</span><span class="sxs-lookup"><span data-stu-id="64548-173">String</span></span>|<span data-ttu-id="64548-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="64548-174">The owner of the app.</span></span> <span data-ttu-id="64548-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-176">developer</span><span class="sxs-lookup"><span data-stu-id="64548-176">developer</span></span>|<span data-ttu-id="64548-177">String</span><span class="sxs-lookup"><span data-stu-id="64548-177">String</span></span>|<span data-ttu-id="64548-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64548-178">The developer of the app.</span></span> <span data-ttu-id="64548-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-180">notes</span><span class="sxs-lookup"><span data-stu-id="64548-180">notes</span></span>|<span data-ttu-id="64548-181">String</span><span class="sxs-lookup"><span data-stu-id="64548-181">String</span></span>|<span data-ttu-id="64548-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64548-182">Notes for the app.</span></span> <span data-ttu-id="64548-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="64548-184">uploadState</span></span>|<span data-ttu-id="64548-185">Int32</span><span class="sxs-lookup"><span data-stu-id="64548-185">Int32</span></span>|<span data-ttu-id="64548-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="64548-186">The upload state.</span></span> <span data-ttu-id="64548-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="64548-188">publishingState</span></span>|[<span data-ttu-id="64548-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="64548-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="64548-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64548-190">The publishing state for the app.</span></span> <span data-ttu-id="64548-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="64548-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="64548-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64548-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="64548-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="64548-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="64548-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="64548-194">isAssigned</span></span>|<span data-ttu-id="64548-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="64548-195">Boolean</span></span>|<span data-ttu-id="64548-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="64548-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="64548-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64548-198">roleScopeTagIds</span></span>|<span data-ttu-id="64548-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="64548-199">String collection</span></span>|<span data-ttu-id="64548-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="64548-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="64548-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="64548-202">dependentAppCount</span></span>|<span data-ttu-id="64548-203">Int32</span><span class="sxs-lookup"><span data-stu-id="64548-203">Int32</span></span>|<span data-ttu-id="64548-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="64548-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="64548-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64548-206">packageId</span><span class="sxs-lookup"><span data-stu-id="64548-206">packageId</span></span>|<span data-ttu-id="64548-207">String</span><span class="sxs-lookup"><span data-stu-id="64548-207">String</span></span>|<span data-ttu-id="64548-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="64548-208">The package identifier.</span></span> <span data-ttu-id="64548-209">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-209">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="64548-210">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="64548-210">appIdentifier</span></span>|<span data-ttu-id="64548-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64548-211">String</span></span>|<span data-ttu-id="64548-212">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="64548-212">The Identity Name.</span></span> <span data-ttu-id="64548-213">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-213">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="64548-214">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="64548-214">usedLicenseCount</span></span>|<span data-ttu-id="64548-215">Int32</span><span class="sxs-lookup"><span data-stu-id="64548-215">Int32</span></span>|<span data-ttu-id="64548-216">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="64548-216">The number of VPP licenses in use.</span></span> <span data-ttu-id="64548-217">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-217">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="64548-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="64548-218">totalLicenseCount</span></span>|<span data-ttu-id="64548-219">Int32</span><span class="sxs-lookup"><span data-stu-id="64548-219">Int32</span></span>|<span data-ttu-id="64548-220">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="64548-220">The total number of VPP licenses.</span></span> <span data-ttu-id="64548-221">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-221">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="64548-222">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="64548-222">appStoreUrl</span></span>|<span data-ttu-id="64548-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64548-223">String</span></span>|<span data-ttu-id="64548-224">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="64548-224">The Play for Work Store app URL.</span></span> <span data-ttu-id="64548-225">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-225">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="64548-226">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="64548-226">isPrivate</span></span>|<span data-ttu-id="64548-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="64548-227">Boolean</span></span>|<span data-ttu-id="64548-228">Indica se o aplicativo está disponível somente para os usuários de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="64548-228">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="64548-229">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-229">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="64548-230">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="64548-230">isSystemApp</span></span>|<span data-ttu-id="64548-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="64548-231">Boolean</span></span>|<span data-ttu-id="64548-232">Indica se o aplicativo é um aplicativo de sistema pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="64548-232">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="64548-233">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-233">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="64548-234">appTracks</span><span class="sxs-lookup"><span data-stu-id="64548-234">appTracks</span></span>|<span data-ttu-id="64548-235">coleção [androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="64548-235">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="64548-236">As faixas que são visíveis para esta empresa.</span><span class="sxs-lookup"><span data-stu-id="64548-236">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="64548-237">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-237">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="64548-238">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="64548-238">supportsOemConfig</span></span>|<span data-ttu-id="64548-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="64548-239">Boolean</span></span>|<span data-ttu-id="64548-240">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="64548-240">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="64548-241">Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="64548-241">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="64548-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="64548-242">Response</span></span>
<span data-ttu-id="64548-243">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64548-243">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64548-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64548-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="64548-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64548-245">Request</span></span>
<span data-ttu-id="64548-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64548-246">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64548-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="64548-247">Response</span></span>
<span data-ttu-id="64548-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64548-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



