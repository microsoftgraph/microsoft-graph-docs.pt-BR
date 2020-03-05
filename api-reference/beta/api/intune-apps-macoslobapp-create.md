---
title: Criar macOSLobApp
description: Criar um novo objeto macOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f20ed7099e66645cf70a3ab01d9c8a0df05e33ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445418"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="8cc59-103">Criar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="8cc59-103">Create macOSLobApp</span></span>

<span data-ttu-id="8cc59-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8cc59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cc59-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cc59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cc59-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cc59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc59-107">Criar um novo objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8cc59-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cc59-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cc59-108">Prerequisites</span></span>
<span data-ttu-id="8cc59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc59-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc59-111">Permission type</span></span>|<span data-ttu-id="8cc59-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cc59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc59-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc59-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc59-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc59-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc59-116">Not supported.</span></span>|
|<span data-ttu-id="8cc59-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc59-117">Application</span></span>|<span data-ttu-id="8cc59-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc59-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc59-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8cc59-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc59-120">Request headers</span></span>
|<span data-ttu-id="8cc59-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cc59-121">Header</span></span>|<span data-ttu-id="8cc59-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8cc59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc59-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc59-123">Authorization</span></span>|<span data-ttu-id="8cc59-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cc59-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cc59-125">Accept</span></span>|<span data-ttu-id="8cc59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc59-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc59-127">Request body</span></span>
<span data-ttu-id="8cc59-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="8cc59-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="8cc59-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="8cc59-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="8cc59-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cc59-130">Property</span></span>|<span data-ttu-id="8cc59-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc59-131">Type</span></span>|<span data-ttu-id="8cc59-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc59-133">id</span><span class="sxs-lookup"><span data-stu-id="8cc59-133">id</span></span>|<span data-ttu-id="8cc59-134">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-134">String</span></span>|<span data-ttu-id="8cc59-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8cc59-135">Key of the entity.</span></span> <span data-ttu-id="8cc59-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8cc59-137">displayName</span></span>|<span data-ttu-id="8cc59-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc59-138">String</span></span>|<span data-ttu-id="8cc59-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8cc59-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8cc59-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-141">description</span><span class="sxs-lookup"><span data-stu-id="8cc59-141">description</span></span>|<span data-ttu-id="8cc59-142">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-142">String</span></span>|<span data-ttu-id="8cc59-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-143">The description of the app.</span></span> <span data-ttu-id="8cc59-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-145">publicador</span><span class="sxs-lookup"><span data-stu-id="8cc59-145">publisher</span></span>|<span data-ttu-id="8cc59-146">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-146">String</span></span>|<span data-ttu-id="8cc59-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-147">The publisher of the app.</span></span> <span data-ttu-id="8cc59-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8cc59-149">largeIcon</span></span>|[<span data-ttu-id="8cc59-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8cc59-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8cc59-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8cc59-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8cc59-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc59-153">createdDateTime</span></span>|<span data-ttu-id="8cc59-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc59-154">DateTimeOffset</span></span>|<span data-ttu-id="8cc59-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-155">The date and time the app was created.</span></span> <span data-ttu-id="8cc59-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc59-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8cc59-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc59-158">DateTimeOffset</span></span>|<span data-ttu-id="8cc59-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8cc59-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8cc59-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8cc59-161">isFeatured</span></span>|<span data-ttu-id="8cc59-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc59-162">Boolean</span></span>|<span data-ttu-id="8cc59-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8cc59-164">privacyInformationUrl</span></span>|<span data-ttu-id="8cc59-165">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-165">String</span></span>|<span data-ttu-id="8cc59-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8cc59-166">The privacy statement Url.</span></span> <span data-ttu-id="8cc59-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8cc59-168">informationUrl</span></span>|<span data-ttu-id="8cc59-169">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-169">String</span></span>|<span data-ttu-id="8cc59-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8cc59-170">The more information Url.</span></span> <span data-ttu-id="8cc59-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-172">owner</span><span class="sxs-lookup"><span data-stu-id="8cc59-172">owner</span></span>|<span data-ttu-id="8cc59-173">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-173">String</span></span>|<span data-ttu-id="8cc59-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-174">The owner of the app.</span></span> <span data-ttu-id="8cc59-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-176">developer</span><span class="sxs-lookup"><span data-stu-id="8cc59-176">developer</span></span>|<span data-ttu-id="8cc59-177">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-177">String</span></span>|<span data-ttu-id="8cc59-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-178">The developer of the app.</span></span> <span data-ttu-id="8cc59-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-180">notes</span><span class="sxs-lookup"><span data-stu-id="8cc59-180">notes</span></span>|<span data-ttu-id="8cc59-181">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-181">String</span></span>|<span data-ttu-id="8cc59-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-182">Notes for the app.</span></span> <span data-ttu-id="8cc59-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8cc59-184">uploadState</span></span>|<span data-ttu-id="8cc59-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc59-185">Int32</span></span>|<span data-ttu-id="8cc59-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="8cc59-186">The upload state.</span></span> <span data-ttu-id="8cc59-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8cc59-188">publishingState</span></span>|[<span data-ttu-id="8cc59-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8cc59-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8cc59-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-190">The publishing state for the app.</span></span> <span data-ttu-id="8cc59-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8cc59-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8cc59-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8cc59-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8cc59-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8cc59-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8cc59-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8cc59-194">isAssigned</span></span>|<span data-ttu-id="8cc59-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc59-195">Boolean</span></span>|<span data-ttu-id="8cc59-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8cc59-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8cc59-198">roleScopeTagIds</span></span>|<span data-ttu-id="8cc59-199">String collection</span><span class="sxs-lookup"><span data-stu-id="8cc59-199">String collection</span></span>|<span data-ttu-id="8cc59-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8cc59-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8cc59-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8cc59-202">dependentAppCount</span></span>|<span data-ttu-id="8cc59-203">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc59-203">Int32</span></span>|<span data-ttu-id="8cc59-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="8cc59-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8cc59-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc59-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8cc59-206">committedContentVersion</span></span>|<span data-ttu-id="8cc59-207">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-207">String</span></span>|<span data-ttu-id="8cc59-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="8cc59-208">The internal committed content version.</span></span> <span data-ttu-id="8cc59-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc59-210">fileName</span><span class="sxs-lookup"><span data-stu-id="8cc59-210">fileName</span></span>|<span data-ttu-id="8cc59-211">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-211">String</span></span>|<span data-ttu-id="8cc59-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="8cc59-212">The name of the main Lob application file.</span></span> <span data-ttu-id="8cc59-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc59-214">size</span><span class="sxs-lookup"><span data-stu-id="8cc59-214">size</span></span>|<span data-ttu-id="8cc59-215">Int64</span><span class="sxs-lookup"><span data-stu-id="8cc59-215">Int64</span></span>|<span data-ttu-id="8cc59-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="8cc59-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="8cc59-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc59-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="8cc59-218">bundleId</span></span>|<span data-ttu-id="8cc59-219">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-219">String</span></span>|<span data-ttu-id="8cc59-220">A ID do pacote.</span><span class="sxs-lookup"><span data-stu-id="8cc59-220">The bundle id.</span></span>|
|<span data-ttu-id="8cc59-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8cc59-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8cc59-222">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8cc59-222">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="8cc59-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8cc59-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8cc59-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="8cc59-224">buildNumber</span></span>|<span data-ttu-id="8cc59-225">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-225">String</span></span>|<span data-ttu-id="8cc59-226">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="8cc59-226">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8cc59-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="8cc59-227">versionNumber</span></span>|<span data-ttu-id="8cc59-228">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-228">String</span></span>|<span data-ttu-id="8cc59-229">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="8cc59-229">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8cc59-230">childApps</span><span class="sxs-lookup"><span data-stu-id="8cc59-230">childApps</span></span>|<span data-ttu-id="8cc59-231">coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc59-231">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="8cc59-232">A lista de aplicativos neste pacote de pacotes</span><span class="sxs-lookup"><span data-stu-id="8cc59-232">The app list in this bundle package</span></span>|
|<span data-ttu-id="8cc59-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8cc59-233">identityVersion</span></span>|<span data-ttu-id="8cc59-234">String</span><span class="sxs-lookup"><span data-stu-id="8cc59-234">String</span></span>|<span data-ttu-id="8cc59-235">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="8cc59-235">The identity version.</span></span>|
|<span data-ttu-id="8cc59-236">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="8cc59-236">md5HashChunkSize</span></span>|<span data-ttu-id="8cc59-237">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc59-237">Int32</span></span>|<span data-ttu-id="8cc59-238">O tamanho da parte do hash MD5</span><span class="sxs-lookup"><span data-stu-id="8cc59-238">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="8cc59-239">md5Hash</span><span class="sxs-lookup"><span data-stu-id="8cc59-239">md5Hash</span></span>|<span data-ttu-id="8cc59-240">String collection</span><span class="sxs-lookup"><span data-stu-id="8cc59-240">String collection</span></span>|<span data-ttu-id="8cc59-241">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="8cc59-241">The MD5 hash codes</span></span>|
|<span data-ttu-id="8cc59-242">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="8cc59-242">ignoreVersionDetection</span></span>|<span data-ttu-id="8cc59-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc59-243">Boolean</span></span>|<span data-ttu-id="8cc59-244">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8cc59-244">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="8cc59-245">Defina isso como true para aplicativos de linha de negócios (LoB) de macOS que usam um recurso de autoatualização.</span><span class="sxs-lookup"><span data-stu-id="8cc59-245">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="8cc59-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc59-246">Response</span></span>
<span data-ttu-id="8cc59-247">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc59-247">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc59-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc59-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cc59-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc59-249">Request</span></span>
<span data-ttu-id="8cc59-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc59-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1616

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="8cc59-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc59-251">Response</span></span>
<span data-ttu-id="8cc59-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc59-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1788

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```





