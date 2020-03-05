---
title: Atualizar androidLobApp
description: Atualiza as propriedades de um objeto androidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27c9e180fb1685527f0f76b8f080ac8a12ac40d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445922"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="2ef28-103">Atualizar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="2ef28-103">Update androidLobApp</span></span>

<span data-ttu-id="2ef28-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ef28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ef28-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ef28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ef28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ef28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ef28-107">Atualiza as propriedades de um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ef28-107">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ef28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ef28-108">Prerequisites</span></span>
<span data-ttu-id="2ef28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ef28-111">Permission type</span></span>|<span data-ttu-id="2ef28-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ef28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ef28-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ef28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ef28-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef28-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ef28-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ef28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ef28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef28-116">Not supported.</span></span>|
|<span data-ttu-id="2ef28-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ef28-117">Application</span></span>|<span data-ttu-id="2ef28-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef28-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ef28-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2ef28-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef28-120">Request headers</span></span>
|<span data-ttu-id="2ef28-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ef28-121">Header</span></span>|<span data-ttu-id="2ef28-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2ef28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ef28-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ef28-123">Authorization</span></span>|<span data-ttu-id="2ef28-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ef28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ef28-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ef28-125">Accept</span></span>|<span data-ttu-id="2ef28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ef28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ef28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef28-127">Request body</span></span>
<span data-ttu-id="2ef28-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ef28-128">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="2ef28-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ef28-129">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="2ef28-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ef28-130">Property</span></span>|<span data-ttu-id="2ef28-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ef28-131">Type</span></span>|<span data-ttu-id="2ef28-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ef28-133">id</span><span class="sxs-lookup"><span data-stu-id="2ef28-133">id</span></span>|<span data-ttu-id="2ef28-134">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-134">String</span></span>|<span data-ttu-id="2ef28-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2ef28-135">Key of the entity.</span></span> <span data-ttu-id="2ef28-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2ef28-137">displayName</span></span>|<span data-ttu-id="2ef28-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ef28-138">String</span></span>|<span data-ttu-id="2ef28-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2ef28-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2ef28-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-141">description</span><span class="sxs-lookup"><span data-stu-id="2ef28-141">description</span></span>|<span data-ttu-id="2ef28-142">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-142">String</span></span>|<span data-ttu-id="2ef28-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ef28-143">The description of the app.</span></span> <span data-ttu-id="2ef28-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-145">publicador</span><span class="sxs-lookup"><span data-stu-id="2ef28-145">publisher</span></span>|<span data-ttu-id="2ef28-146">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-146">String</span></span>|<span data-ttu-id="2ef28-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ef28-147">The publisher of the app.</span></span> <span data-ttu-id="2ef28-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2ef28-149">largeIcon</span></span>|[<span data-ttu-id="2ef28-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2ef28-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2ef28-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2ef28-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2ef28-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ef28-153">createdDateTime</span></span>|<span data-ttu-id="2ef28-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ef28-154">DateTimeOffset</span></span>|<span data-ttu-id="2ef28-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ef28-155">The date and time the app was created.</span></span> <span data-ttu-id="2ef28-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ef28-157">lastModifiedDateTime</span></span>|<span data-ttu-id="2ef28-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ef28-158">DateTimeOffset</span></span>|<span data-ttu-id="2ef28-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2ef28-159">The date and time the app was last modified.</span></span> <span data-ttu-id="2ef28-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2ef28-161">isFeatured</span></span>|<span data-ttu-id="2ef28-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ef28-162">Boolean</span></span>|<span data-ttu-id="2ef28-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2ef28-164">privacyInformationUrl</span></span>|<span data-ttu-id="2ef28-165">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-165">String</span></span>|<span data-ttu-id="2ef28-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2ef28-166">The privacy statement Url.</span></span> <span data-ttu-id="2ef28-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2ef28-168">informationUrl</span></span>|<span data-ttu-id="2ef28-169">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-169">String</span></span>|<span data-ttu-id="2ef28-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2ef28-170">The more information Url.</span></span> <span data-ttu-id="2ef28-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-172">owner</span><span class="sxs-lookup"><span data-stu-id="2ef28-172">owner</span></span>|<span data-ttu-id="2ef28-173">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-173">String</span></span>|<span data-ttu-id="2ef28-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2ef28-174">The owner of the app.</span></span> <span data-ttu-id="2ef28-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-176">developer</span><span class="sxs-lookup"><span data-stu-id="2ef28-176">developer</span></span>|<span data-ttu-id="2ef28-177">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-177">String</span></span>|<span data-ttu-id="2ef28-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ef28-178">The developer of the app.</span></span> <span data-ttu-id="2ef28-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-180">notes</span><span class="sxs-lookup"><span data-stu-id="2ef28-180">notes</span></span>|<span data-ttu-id="2ef28-181">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-181">String</span></span>|<span data-ttu-id="2ef28-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ef28-182">Notes for the app.</span></span> <span data-ttu-id="2ef28-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="2ef28-184">uploadState</span></span>|<span data-ttu-id="2ef28-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2ef28-185">Int32</span></span>|<span data-ttu-id="2ef28-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="2ef28-186">The upload state.</span></span> <span data-ttu-id="2ef28-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="2ef28-188">publishingState</span></span>|[<span data-ttu-id="2ef28-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2ef28-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2ef28-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ef28-190">The publishing state for the app.</span></span> <span data-ttu-id="2ef28-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2ef28-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2ef28-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ef28-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2ef28-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2ef28-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2ef28-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2ef28-194">isAssigned</span></span>|<span data-ttu-id="2ef28-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ef28-195">Boolean</span></span>|<span data-ttu-id="2ef28-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="2ef28-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2ef28-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ef28-198">roleScopeTagIds</span></span>|<span data-ttu-id="2ef28-199">String collection</span><span class="sxs-lookup"><span data-stu-id="2ef28-199">String collection</span></span>|<span data-ttu-id="2ef28-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2ef28-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2ef28-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="2ef28-202">dependentAppCount</span></span>|<span data-ttu-id="2ef28-203">Int32</span><span class="sxs-lookup"><span data-stu-id="2ef28-203">Int32</span></span>|<span data-ttu-id="2ef28-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="2ef28-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2ef28-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ef28-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2ef28-206">committedContentVersion</span></span>|<span data-ttu-id="2ef28-207">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-207">String</span></span>|<span data-ttu-id="2ef28-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="2ef28-208">The internal committed content version.</span></span> <span data-ttu-id="2ef28-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2ef28-210">fileName</span><span class="sxs-lookup"><span data-stu-id="2ef28-210">fileName</span></span>|<span data-ttu-id="2ef28-211">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-211">String</span></span>|<span data-ttu-id="2ef28-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="2ef28-212">The name of the main Lob application file.</span></span> <span data-ttu-id="2ef28-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2ef28-214">size</span><span class="sxs-lookup"><span data-stu-id="2ef28-214">size</span></span>|<span data-ttu-id="2ef28-215">Int64</span><span class="sxs-lookup"><span data-stu-id="2ef28-215">Int64</span></span>|<span data-ttu-id="2ef28-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="2ef28-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="2ef28-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ef28-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2ef28-218">packageId</span><span class="sxs-lookup"><span data-stu-id="2ef28-218">packageId</span></span>|<span data-ttu-id="2ef28-219">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-219">String</span></span>|<span data-ttu-id="2ef28-220">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="2ef28-220">The package identifier.</span></span>|
|<span data-ttu-id="2ef28-221">identityName</span><span class="sxs-lookup"><span data-stu-id="2ef28-221">identityName</span></span>|<span data-ttu-id="2ef28-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ef28-222">String</span></span>|<span data-ttu-id="2ef28-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="2ef28-223">The Identity Name.</span></span>|
|<span data-ttu-id="2ef28-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ef28-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2ef28-225">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ef28-225">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="2ef28-226">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="2ef28-226">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2ef28-227">versionName</span><span class="sxs-lookup"><span data-stu-id="2ef28-227">versionName</span></span>|<span data-ttu-id="2ef28-228">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-228">String</span></span>|<span data-ttu-id="2ef28-229">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="2ef28-229">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2ef28-230">versionCode</span><span class="sxs-lookup"><span data-stu-id="2ef28-230">versionCode</span></span>|<span data-ttu-id="2ef28-231">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-231">String</span></span>|<span data-ttu-id="2ef28-232">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="2ef28-232">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2ef28-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2ef28-233">identityVersion</span></span>|<span data-ttu-id="2ef28-234">String</span><span class="sxs-lookup"><span data-stu-id="2ef28-234">String</span></span>|<span data-ttu-id="2ef28-235">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="2ef28-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2ef28-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef28-236">Response</span></span>
<span data-ttu-id="2ef28-237">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef28-237">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef28-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ef28-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ef28-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef28-239">Request</span></span>
<span data-ttu-id="2ef28-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ef28-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="2ef28-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef28-241">Response</span></span>
<span data-ttu-id="2ef28-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ef28-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





