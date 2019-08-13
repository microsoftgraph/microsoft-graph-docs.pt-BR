---
title: Criar androidStoreApp
description: Criar um novo objeto androidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e421713363242dc8b8f77a2db4d65d4c67c4a86a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331053"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="0f61c-103">Criar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="0f61c-103">Create androidStoreApp</span></span>

> <span data-ttu-id="0f61c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f61c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f61c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f61c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f61c-106">Criar um novo objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f61c-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f61c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f61c-107">Prerequisites</span></span>
<span data-ttu-id="0f61c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f61c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f61c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f61c-110">Permission type</span></span>|<span data-ttu-id="0f61c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f61c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f61c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f61c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f61c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f61c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f61c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f61c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f61c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f61c-115">Not supported.</span></span>|
|<span data-ttu-id="0f61c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f61c-116">Application</span></span>|<span data-ttu-id="0f61c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f61c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f61c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f61c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0f61c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f61c-119">Request headers</span></span>
|<span data-ttu-id="0f61c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f61c-120">Header</span></span>|<span data-ttu-id="0f61c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0f61c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f61c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f61c-122">Authorization</span></span>|<span data-ttu-id="0f61c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f61c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f61c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f61c-124">Accept</span></span>|<span data-ttu-id="0f61c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f61c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f61c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f61c-126">Request body</span></span>
<span data-ttu-id="0f61c-127">No corpo da solicitação, forneça uma representação JSON do objeto androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="0f61c-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="0f61c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="0f61c-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="0f61c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f61c-129">Property</span></span>|<span data-ttu-id="0f61c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f61c-130">Type</span></span>|<span data-ttu-id="0f61c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f61c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f61c-132">id</span><span class="sxs-lookup"><span data-stu-id="0f61c-132">id</span></span>|<span data-ttu-id="0f61c-133">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-133">String</span></span>|<span data-ttu-id="0f61c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f61c-134">Key of the entity.</span></span> <span data-ttu-id="0f61c-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0f61c-136">displayName</span></span>|<span data-ttu-id="0f61c-137">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-137">String</span></span>|<span data-ttu-id="0f61c-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0f61c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0f61c-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-140">descrição</span><span class="sxs-lookup"><span data-stu-id="0f61c-140">description</span></span>|<span data-ttu-id="0f61c-141">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-141">String</span></span>|<span data-ttu-id="0f61c-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f61c-142">The description of the app.</span></span> <span data-ttu-id="0f61c-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-144">publicador</span><span class="sxs-lookup"><span data-stu-id="0f61c-144">publisher</span></span>|<span data-ttu-id="0f61c-145">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-145">String</span></span>|<span data-ttu-id="0f61c-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f61c-146">The publisher of the app.</span></span> <span data-ttu-id="0f61c-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0f61c-148">largeIcon</span></span>|[<span data-ttu-id="0f61c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f61c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f61c-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0f61c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0f61c-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f61c-152">createdDateTime</span></span>|<span data-ttu-id="0f61c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f61c-153">DateTimeOffset</span></span>|<span data-ttu-id="0f61c-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f61c-154">The date and time the app was created.</span></span> <span data-ttu-id="0f61c-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f61c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0f61c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f61c-157">DateTimeOffset</span></span>|<span data-ttu-id="0f61c-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0f61c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0f61c-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0f61c-160">isFeatured</span></span>|<span data-ttu-id="0f61c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f61c-161">Boolean</span></span>|<span data-ttu-id="0f61c-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0f61c-163">privacyInformationUrl</span></span>|<span data-ttu-id="0f61c-164">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-164">String</span></span>|<span data-ttu-id="0f61c-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0f61c-165">The privacy statement Url.</span></span> <span data-ttu-id="0f61c-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0f61c-167">informationUrl</span></span>|<span data-ttu-id="0f61c-168">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-168">String</span></span>|<span data-ttu-id="0f61c-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0f61c-169">The more information Url.</span></span> <span data-ttu-id="0f61c-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-171">owner</span><span class="sxs-lookup"><span data-stu-id="0f61c-171">owner</span></span>|<span data-ttu-id="0f61c-172">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-172">String</span></span>|<span data-ttu-id="0f61c-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0f61c-173">The owner of the app.</span></span> <span data-ttu-id="0f61c-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-175">developer</span><span class="sxs-lookup"><span data-stu-id="0f61c-175">developer</span></span>|<span data-ttu-id="0f61c-176">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-176">String</span></span>|<span data-ttu-id="0f61c-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f61c-177">The developer of the app.</span></span> <span data-ttu-id="0f61c-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-179">notes</span><span class="sxs-lookup"><span data-stu-id="0f61c-179">notes</span></span>|<span data-ttu-id="0f61c-180">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-180">String</span></span>|<span data-ttu-id="0f61c-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f61c-181">Notes for the app.</span></span> <span data-ttu-id="0f61c-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0f61c-183">uploadState</span></span>|<span data-ttu-id="0f61c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0f61c-184">Int32</span></span>|<span data-ttu-id="0f61c-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="0f61c-185">The upload state.</span></span> <span data-ttu-id="0f61c-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0f61c-187">publishingState</span></span>|[<span data-ttu-id="0f61c-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0f61c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0f61c-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f61c-189">The publishing state for the app.</span></span> <span data-ttu-id="0f61c-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0f61c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0f61c-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f61c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0f61c-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0f61c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0f61c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0f61c-193">isAssigned</span></span>|<span data-ttu-id="0f61c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f61c-194">Boolean</span></span>|<span data-ttu-id="0f61c-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="0f61c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0f61c-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f61c-197">roleScopeTagIds</span></span>|<span data-ttu-id="0f61c-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f61c-198">String collection</span></span>|<span data-ttu-id="0f61c-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0f61c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0f61c-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0f61c-201">dependentAppCount</span></span>|<span data-ttu-id="0f61c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="0f61c-202">Int32</span></span>|<span data-ttu-id="0f61c-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="0f61c-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0f61c-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f61c-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f61c-205">packageId</span><span class="sxs-lookup"><span data-stu-id="0f61c-205">packageId</span></span>|<span data-ttu-id="0f61c-206">String</span><span class="sxs-lookup"><span data-stu-id="0f61c-206">String</span></span>|<span data-ttu-id="0f61c-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="0f61c-207">The package identifier.</span></span>|
|<span data-ttu-id="0f61c-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="0f61c-208">appIdentifier</span></span>|<span data-ttu-id="0f61c-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f61c-209">String</span></span>|<span data-ttu-id="0f61c-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0f61c-210">The Identity Name.</span></span>|
|<span data-ttu-id="0f61c-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0f61c-211">appStoreUrl</span></span>|<span data-ttu-id="0f61c-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f61c-212">String</span></span>|<span data-ttu-id="0f61c-213">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="0f61c-213">The Android app store URL.</span></span>|
|<span data-ttu-id="0f61c-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f61c-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0f61c-215">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f61c-215">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="0f61c-216">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="0f61c-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0f61c-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f61c-217">Response</span></span>
<span data-ttu-id="0f61c-218">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f61c-218">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f61c-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f61c-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f61c-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f61c-220">Request</span></span>
<span data-ttu-id="0f61c-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f61c-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1230

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="0f61c-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f61c-222">Response</span></span>
<span data-ttu-id="0f61c-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f61c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1402

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```






