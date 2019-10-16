---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12d7d02cedef0a99f477bea5f4cb7fd5caf946ae
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535531"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="2bcba-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="2bcba-103">Create androidLobApp</span></span>

> <span data-ttu-id="2bcba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bcba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bcba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bcba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bcba-106">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2bcba-106">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bcba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bcba-107">Prerequisites</span></span>
<span data-ttu-id="2bcba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bcba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bcba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bcba-110">Permission type</span></span>|<span data-ttu-id="2bcba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bcba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bcba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bcba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bcba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bcba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2bcba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bcba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bcba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bcba-115">Not supported.</span></span>|
|<span data-ttu-id="2bcba-116">Application</span><span class="sxs-lookup"><span data-stu-id="2bcba-116">Application</span></span>|<span data-ttu-id="2bcba-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bcba-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bcba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bcba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2bcba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bcba-119">Request headers</span></span>
|<span data-ttu-id="2bcba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bcba-120">Header</span></span>|<span data-ttu-id="2bcba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2bcba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bcba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bcba-122">Authorization</span></span>|<span data-ttu-id="2bcba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bcba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bcba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bcba-124">Accept</span></span>|<span data-ttu-id="2bcba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bcba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bcba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bcba-126">Request body</span></span>
<span data-ttu-id="2bcba-127">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="2bcba-127">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="2bcba-128">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="2bcba-128">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="2bcba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bcba-129">Property</span></span>|<span data-ttu-id="2bcba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bcba-130">Type</span></span>|<span data-ttu-id="2bcba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bcba-132">id</span><span class="sxs-lookup"><span data-stu-id="2bcba-132">id</span></span>|<span data-ttu-id="2bcba-133">String</span><span class="sxs-lookup"><span data-stu-id="2bcba-133">String</span></span>|<span data-ttu-id="2bcba-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2bcba-134">Key of the entity.</span></span> <span data-ttu-id="2bcba-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2bcba-136">displayName</span></span>|<span data-ttu-id="2bcba-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-137">String</span></span>|<span data-ttu-id="2bcba-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2bcba-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2bcba-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-140">description</span><span class="sxs-lookup"><span data-stu-id="2bcba-140">description</span></span>|<span data-ttu-id="2bcba-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-141">String</span></span>|<span data-ttu-id="2bcba-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2bcba-142">The description of the app.</span></span> <span data-ttu-id="2bcba-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-144">publicador</span><span class="sxs-lookup"><span data-stu-id="2bcba-144">publisher</span></span>|<span data-ttu-id="2bcba-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-145">String</span></span>|<span data-ttu-id="2bcba-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2bcba-146">The publisher of the app.</span></span> <span data-ttu-id="2bcba-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2bcba-148">largeIcon</span></span>|[<span data-ttu-id="2bcba-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2bcba-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2bcba-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2bcba-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2bcba-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bcba-152">createdDateTime</span></span>|<span data-ttu-id="2bcba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bcba-153">DateTimeOffset</span></span>|<span data-ttu-id="2bcba-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2bcba-154">The date and time the app was created.</span></span> <span data-ttu-id="2bcba-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bcba-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2bcba-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bcba-157">DateTimeOffset</span></span>|<span data-ttu-id="2bcba-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2bcba-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2bcba-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2bcba-160">isFeatured</span></span>|<span data-ttu-id="2bcba-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcba-161">Boolean</span></span>|<span data-ttu-id="2bcba-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2bcba-163">privacyInformationUrl</span></span>|<span data-ttu-id="2bcba-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-164">String</span></span>|<span data-ttu-id="2bcba-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2bcba-165">The privacy statement Url.</span></span> <span data-ttu-id="2bcba-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2bcba-167">informationUrl</span></span>|<span data-ttu-id="2bcba-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-168">String</span></span>|<span data-ttu-id="2bcba-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2bcba-169">The more information Url.</span></span> <span data-ttu-id="2bcba-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-171">owner</span><span class="sxs-lookup"><span data-stu-id="2bcba-171">owner</span></span>|<span data-ttu-id="2bcba-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-172">String</span></span>|<span data-ttu-id="2bcba-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2bcba-173">The owner of the app.</span></span> <span data-ttu-id="2bcba-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-175">developer</span><span class="sxs-lookup"><span data-stu-id="2bcba-175">developer</span></span>|<span data-ttu-id="2bcba-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-176">String</span></span>|<span data-ttu-id="2bcba-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2bcba-177">The developer of the app.</span></span> <span data-ttu-id="2bcba-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-179">notes</span><span class="sxs-lookup"><span data-stu-id="2bcba-179">notes</span></span>|<span data-ttu-id="2bcba-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-180">String</span></span>|<span data-ttu-id="2bcba-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2bcba-181">Notes for the app.</span></span> <span data-ttu-id="2bcba-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2bcba-183">uploadState</span></span>|<span data-ttu-id="2bcba-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2bcba-184">Int32</span></span>|<span data-ttu-id="2bcba-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="2bcba-185">The upload state.</span></span> <span data-ttu-id="2bcba-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2bcba-187">publishingState</span></span>|[<span data-ttu-id="2bcba-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2bcba-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2bcba-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2bcba-189">The publishing state for the app.</span></span> <span data-ttu-id="2bcba-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2bcba-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2bcba-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2bcba-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2bcba-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2bcba-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2bcba-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2bcba-193">isAssigned</span></span>|<span data-ttu-id="2bcba-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bcba-194">Boolean</span></span>|<span data-ttu-id="2bcba-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="2bcba-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2bcba-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2bcba-197">roleScopeTagIds</span></span>|<span data-ttu-id="2bcba-198">String collection</span><span class="sxs-lookup"><span data-stu-id="2bcba-198">String collection</span></span>|<span data-ttu-id="2bcba-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2bcba-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2bcba-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="2bcba-201">dependentAppCount</span></span>|<span data-ttu-id="2bcba-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2bcba-202">Int32</span></span>|<span data-ttu-id="2bcba-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="2bcba-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2bcba-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2bcba-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2bcba-205">committedContentVersion</span></span>|<span data-ttu-id="2bcba-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-206">String</span></span>|<span data-ttu-id="2bcba-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="2bcba-207">The internal committed content version.</span></span> <span data-ttu-id="2bcba-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2bcba-209">fileName</span><span class="sxs-lookup"><span data-stu-id="2bcba-209">fileName</span></span>|<span data-ttu-id="2bcba-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-210">String</span></span>|<span data-ttu-id="2bcba-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="2bcba-211">The name of the main Lob application file.</span></span> <span data-ttu-id="2bcba-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2bcba-213">size</span><span class="sxs-lookup"><span data-stu-id="2bcba-213">size</span></span>|<span data-ttu-id="2bcba-214">Int64</span><span class="sxs-lookup"><span data-stu-id="2bcba-214">Int64</span></span>|<span data-ttu-id="2bcba-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="2bcba-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="2bcba-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bcba-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2bcba-217">packageId</span><span class="sxs-lookup"><span data-stu-id="2bcba-217">packageId</span></span>|<span data-ttu-id="2bcba-218">String</span><span class="sxs-lookup"><span data-stu-id="2bcba-218">String</span></span>|<span data-ttu-id="2bcba-219">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="2bcba-219">The package identifier.</span></span>|
|<span data-ttu-id="2bcba-220">identityName</span><span class="sxs-lookup"><span data-stu-id="2bcba-220">identityName</span></span>|<span data-ttu-id="2bcba-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-221">String</span></span>|<span data-ttu-id="2bcba-222">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="2bcba-222">The Identity Name.</span></span>|
|<span data-ttu-id="2bcba-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2bcba-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2bcba-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2bcba-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="2bcba-225">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="2bcba-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2bcba-226">versionName</span><span class="sxs-lookup"><span data-stu-id="2bcba-226">versionName</span></span>|<span data-ttu-id="2bcba-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-227">String</span></span>|<span data-ttu-id="2bcba-228">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="2bcba-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2bcba-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="2bcba-229">versionCode</span></span>|<span data-ttu-id="2bcba-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcba-230">String</span></span>|<span data-ttu-id="2bcba-231">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="2bcba-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2bcba-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2bcba-232">identityVersion</span></span>|<span data-ttu-id="2bcba-233">String</span><span class="sxs-lookup"><span data-stu-id="2bcba-233">String</span></span>|<span data-ttu-id="2bcba-234">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="2bcba-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2bcba-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bcba-235">Response</span></span>
<span data-ttu-id="2bcba-236">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bcba-236">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bcba-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bcba-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bcba-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bcba-238">Request</span></span>
<span data-ttu-id="2bcba-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bcba-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="2bcba-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bcba-240">Response</span></span>
<span data-ttu-id="2bcba-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bcba-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```






