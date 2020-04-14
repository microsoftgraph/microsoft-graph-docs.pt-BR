---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00310232a4ba1a35825f42ad63ecdbb080b15024
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395231"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="f2a31-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="f2a31-103">Create androidLobApp</span></span>

<span data-ttu-id="f2a31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2a31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2a31-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2a31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2a31-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2a31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2a31-107">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2a31-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2a31-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2a31-108">Prerequisites</span></span>
<span data-ttu-id="f2a31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2a31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2a31-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2a31-111">Permission type</span></span>|<span data-ttu-id="f2a31-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2a31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2a31-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2a31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2a31-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2a31-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2a31-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2a31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2a31-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2a31-116">Not supported.</span></span>|
|<span data-ttu-id="f2a31-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2a31-117">Application</span></span>|<span data-ttu-id="f2a31-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2a31-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2a31-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2a31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f2a31-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a31-120">Request headers</span></span>
|<span data-ttu-id="f2a31-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2a31-121">Header</span></span>|<span data-ttu-id="f2a31-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2a31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2a31-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2a31-123">Authorization</span></span>|<span data-ttu-id="f2a31-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2a31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2a31-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2a31-125">Accept</span></span>|<span data-ttu-id="f2a31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2a31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2a31-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a31-127">Request body</span></span>
<span data-ttu-id="f2a31-128">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="f2a31-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="f2a31-129">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="f2a31-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="f2a31-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2a31-130">Property</span></span>|<span data-ttu-id="f2a31-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2a31-131">Type</span></span>|<span data-ttu-id="f2a31-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2a31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2a31-133">id</span><span class="sxs-lookup"><span data-stu-id="f2a31-133">id</span></span>|<span data-ttu-id="f2a31-134">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-134">String</span></span>|<span data-ttu-id="f2a31-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2a31-135">Key of the entity.</span></span> <span data-ttu-id="f2a31-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f2a31-137">displayName</span></span>|<span data-ttu-id="f2a31-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2a31-138">String</span></span>|<span data-ttu-id="f2a31-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f2a31-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2a31-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-141">description</span><span class="sxs-lookup"><span data-stu-id="f2a31-141">description</span></span>|<span data-ttu-id="f2a31-142">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-142">String</span></span>|<span data-ttu-id="f2a31-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a31-143">The description of the app.</span></span> <span data-ttu-id="f2a31-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-145">publicador</span><span class="sxs-lookup"><span data-stu-id="f2a31-145">publisher</span></span>|<span data-ttu-id="f2a31-146">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-146">String</span></span>|<span data-ttu-id="f2a31-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a31-147">The publisher of the app.</span></span> <span data-ttu-id="f2a31-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2a31-149">largeIcon</span></span>|[<span data-ttu-id="f2a31-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2a31-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2a31-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f2a31-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2a31-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2a31-153">createdDateTime</span></span>|<span data-ttu-id="f2a31-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2a31-154">DateTimeOffset</span></span>|<span data-ttu-id="f2a31-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a31-155">The date and time the app was created.</span></span> <span data-ttu-id="f2a31-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2a31-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f2a31-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2a31-158">DateTimeOffset</span></span>|<span data-ttu-id="f2a31-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f2a31-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f2a31-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2a31-161">isFeatured</span></span>|<span data-ttu-id="f2a31-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2a31-162">Boolean</span></span>|<span data-ttu-id="f2a31-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2a31-164">privacyInformationUrl</span></span>|<span data-ttu-id="f2a31-165">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-165">String</span></span>|<span data-ttu-id="f2a31-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f2a31-166">The privacy statement Url.</span></span> <span data-ttu-id="f2a31-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2a31-168">informationUrl</span></span>|<span data-ttu-id="f2a31-169">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-169">String</span></span>|<span data-ttu-id="f2a31-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f2a31-170">The more information Url.</span></span> <span data-ttu-id="f2a31-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-172">owner</span><span class="sxs-lookup"><span data-stu-id="f2a31-172">owner</span></span>|<span data-ttu-id="f2a31-173">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-173">String</span></span>|<span data-ttu-id="f2a31-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f2a31-174">The owner of the app.</span></span> <span data-ttu-id="f2a31-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-176">developer</span><span class="sxs-lookup"><span data-stu-id="f2a31-176">developer</span></span>|<span data-ttu-id="f2a31-177">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-177">String</span></span>|<span data-ttu-id="f2a31-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a31-178">The developer of the app.</span></span> <span data-ttu-id="f2a31-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-180">notes</span><span class="sxs-lookup"><span data-stu-id="f2a31-180">notes</span></span>|<span data-ttu-id="f2a31-181">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-181">String</span></span>|<span data-ttu-id="f2a31-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a31-182">Notes for the app.</span></span> <span data-ttu-id="f2a31-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2a31-184">uploadState</span></span>|<span data-ttu-id="f2a31-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a31-185">Int32</span></span>|<span data-ttu-id="f2a31-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="f2a31-186">The upload state.</span></span> <span data-ttu-id="f2a31-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2a31-188">publishingState</span></span>|[<span data-ttu-id="f2a31-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2a31-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2a31-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a31-190">The publishing state for the app.</span></span> <span data-ttu-id="f2a31-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f2a31-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2a31-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2a31-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f2a31-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f2a31-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2a31-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f2a31-194">isAssigned</span></span>|<span data-ttu-id="f2a31-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2a31-195">Boolean</span></span>|<span data-ttu-id="f2a31-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f2a31-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f2a31-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2a31-198">roleScopeTagIds</span></span>|<span data-ttu-id="f2a31-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f2a31-199">String collection</span></span>|<span data-ttu-id="f2a31-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f2a31-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f2a31-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f2a31-202">dependentAppCount</span></span>|<span data-ttu-id="f2a31-203">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a31-203">Int32</span></span>|<span data-ttu-id="f2a31-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="f2a31-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f2a31-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a31-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f2a31-206">committedContentVersion</span></span>|<span data-ttu-id="f2a31-207">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-207">String</span></span>|<span data-ttu-id="f2a31-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f2a31-208">The internal committed content version.</span></span> <span data-ttu-id="f2a31-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2a31-210">fileName</span><span class="sxs-lookup"><span data-stu-id="f2a31-210">fileName</span></span>|<span data-ttu-id="f2a31-211">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-211">String</span></span>|<span data-ttu-id="f2a31-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f2a31-212">The name of the main Lob application file.</span></span> <span data-ttu-id="f2a31-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2a31-214">size</span><span class="sxs-lookup"><span data-stu-id="f2a31-214">size</span></span>|<span data-ttu-id="f2a31-215">Int64</span><span class="sxs-lookup"><span data-stu-id="f2a31-215">Int64</span></span>|<span data-ttu-id="f2a31-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f2a31-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="f2a31-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a31-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2a31-218">packageId</span><span class="sxs-lookup"><span data-stu-id="f2a31-218">packageId</span></span>|<span data-ttu-id="f2a31-219">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-219">String</span></span>|<span data-ttu-id="f2a31-220">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="f2a31-220">The package identifier.</span></span>|
|<span data-ttu-id="f2a31-221">identityName</span><span class="sxs-lookup"><span data-stu-id="f2a31-221">identityName</span></span>|<span data-ttu-id="f2a31-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2a31-222">String</span></span>|<span data-ttu-id="f2a31-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f2a31-223">The Identity Name.</span></span>|
|<span data-ttu-id="f2a31-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2a31-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f2a31-225">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2a31-225">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f2a31-226">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f2a31-226">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f2a31-227">versionName</span><span class="sxs-lookup"><span data-stu-id="f2a31-227">versionName</span></span>|<span data-ttu-id="f2a31-228">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-228">String</span></span>|<span data-ttu-id="f2a31-229">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="f2a31-229">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f2a31-230">versionCode</span><span class="sxs-lookup"><span data-stu-id="f2a31-230">versionCode</span></span>|<span data-ttu-id="f2a31-231">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-231">String</span></span>|<span data-ttu-id="f2a31-232">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="f2a31-232">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f2a31-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f2a31-233">identityVersion</span></span>|<span data-ttu-id="f2a31-234">String</span><span class="sxs-lookup"><span data-stu-id="f2a31-234">String</span></span>|<span data-ttu-id="f2a31-235">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="f2a31-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f2a31-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a31-236">Response</span></span>
<span data-ttu-id="f2a31-237">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2a31-237">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2a31-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2a31-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2a31-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a31-239">Request</span></span>
<span data-ttu-id="f2a31-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2a31-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2a31-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a31-241">Response</span></span>
<span data-ttu-id="f2a31-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2a31-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



