---
title: Criar win32LobApp
description: Criar um novo objeto win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f04026f65c32097296ffbbb610d71be7e4bef99f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450598"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="32c4b-103">Criar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="32c4b-103">Create win32LobApp</span></span>

<span data-ttu-id="32c4b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32c4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32c4b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32c4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32c4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32c4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32c4b-107">Criar um novo objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="32c4b-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32c4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32c4b-108">Prerequisites</span></span>
<span data-ttu-id="32c4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32c4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32c4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32c4b-111">Permission type</span></span>|<span data-ttu-id="32c4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32c4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32c4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32c4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32c4b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c4b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32c4b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32c4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32c4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32c4b-116">Not supported.</span></span>|
|<span data-ttu-id="32c4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32c4b-117">Application</span></span>|<span data-ttu-id="32c4b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c4b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32c4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32c4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="32c4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32c4b-120">Request headers</span></span>
|<span data-ttu-id="32c4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32c4b-121">Header</span></span>|<span data-ttu-id="32c4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="32c4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32c4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32c4b-123">Authorization</span></span>|<span data-ttu-id="32c4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32c4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32c4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32c4b-125">Accept</span></span>|<span data-ttu-id="32c4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32c4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32c4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32c4b-127">Request body</span></span>
<span data-ttu-id="32c4b-128">No corpo da solicitação, forneça uma representação JSON do objeto win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="32c4b-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="32c4b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="32c4b-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="32c4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32c4b-130">Property</span></span>|<span data-ttu-id="32c4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="32c4b-131">Type</span></span>|<span data-ttu-id="32c4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="32c4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32c4b-133">id</span><span class="sxs-lookup"><span data-stu-id="32c4b-133">id</span></span>|<span data-ttu-id="32c4b-134">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-134">String</span></span>|<span data-ttu-id="32c4b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="32c4b-135">Key of the entity.</span></span> <span data-ttu-id="32c4b-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="32c4b-137">displayName</span></span>|<span data-ttu-id="32c4b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32c4b-138">String</span></span>|<span data-ttu-id="32c4b-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="32c4b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="32c4b-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-141">description</span><span class="sxs-lookup"><span data-stu-id="32c4b-141">description</span></span>|<span data-ttu-id="32c4b-142">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-142">String</span></span>|<span data-ttu-id="32c4b-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-143">The description of the app.</span></span> <span data-ttu-id="32c4b-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-145">publicador</span><span class="sxs-lookup"><span data-stu-id="32c4b-145">publisher</span></span>|<span data-ttu-id="32c4b-146">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-146">String</span></span>|<span data-ttu-id="32c4b-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-147">The publisher of the app.</span></span> <span data-ttu-id="32c4b-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="32c4b-149">largeIcon</span></span>|[<span data-ttu-id="32c4b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="32c4b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="32c4b-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="32c4b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="32c4b-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32c4b-153">createdDateTime</span></span>|<span data-ttu-id="32c4b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32c4b-154">DateTimeOffset</span></span>|<span data-ttu-id="32c4b-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-155">The date and time the app was created.</span></span> <span data-ttu-id="32c4b-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32c4b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="32c4b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32c4b-158">DateTimeOffset</span></span>|<span data-ttu-id="32c4b-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="32c4b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="32c4b-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="32c4b-161">isFeatured</span></span>|<span data-ttu-id="32c4b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="32c4b-162">Boolean</span></span>|<span data-ttu-id="32c4b-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="32c4b-164">privacyInformationUrl</span></span>|<span data-ttu-id="32c4b-165">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-165">String</span></span>|<span data-ttu-id="32c4b-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="32c4b-166">The privacy statement Url.</span></span> <span data-ttu-id="32c4b-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="32c4b-168">informationUrl</span></span>|<span data-ttu-id="32c4b-169">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-169">String</span></span>|<span data-ttu-id="32c4b-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="32c4b-170">The more information Url.</span></span> <span data-ttu-id="32c4b-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-172">owner</span><span class="sxs-lookup"><span data-stu-id="32c4b-172">owner</span></span>|<span data-ttu-id="32c4b-173">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-173">String</span></span>|<span data-ttu-id="32c4b-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-174">The owner of the app.</span></span> <span data-ttu-id="32c4b-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-176">developer</span><span class="sxs-lookup"><span data-stu-id="32c4b-176">developer</span></span>|<span data-ttu-id="32c4b-177">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-177">String</span></span>|<span data-ttu-id="32c4b-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-178">The developer of the app.</span></span> <span data-ttu-id="32c4b-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-180">notes</span><span class="sxs-lookup"><span data-stu-id="32c4b-180">notes</span></span>|<span data-ttu-id="32c4b-181">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-181">String</span></span>|<span data-ttu-id="32c4b-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-182">Notes for the app.</span></span> <span data-ttu-id="32c4b-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="32c4b-184">uploadState</span></span>|<span data-ttu-id="32c4b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="32c4b-185">Int32</span></span>|<span data-ttu-id="32c4b-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="32c4b-186">The upload state.</span></span> <span data-ttu-id="32c4b-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="32c4b-188">publishingState</span></span>|[<span data-ttu-id="32c4b-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="32c4b-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="32c4b-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-190">The publishing state for the app.</span></span> <span data-ttu-id="32c4b-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="32c4b-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="32c4b-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32c4b-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="32c4b-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="32c4b-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="32c4b-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="32c4b-194">isAssigned</span></span>|<span data-ttu-id="32c4b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="32c4b-195">Boolean</span></span>|<span data-ttu-id="32c4b-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="32c4b-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="32c4b-198">roleScopeTagIds</span></span>|<span data-ttu-id="32c4b-199">String collection</span><span class="sxs-lookup"><span data-stu-id="32c4b-199">String collection</span></span>|<span data-ttu-id="32c4b-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="32c4b-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="32c4b-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="32c4b-202">dependentAppCount</span></span>|<span data-ttu-id="32c4b-203">Int32</span><span class="sxs-lookup"><span data-stu-id="32c4b-203">Int32</span></span>|<span data-ttu-id="32c4b-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="32c4b-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="32c4b-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32c4b-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="32c4b-206">committedContentVersion</span></span>|<span data-ttu-id="32c4b-207">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-207">String</span></span>|<span data-ttu-id="32c4b-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="32c4b-208">The internal committed content version.</span></span> <span data-ttu-id="32c4b-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="32c4b-210">fileName</span><span class="sxs-lookup"><span data-stu-id="32c4b-210">fileName</span></span>|<span data-ttu-id="32c4b-211">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-211">String</span></span>|<span data-ttu-id="32c4b-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="32c4b-212">The name of the main Lob application file.</span></span> <span data-ttu-id="32c4b-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="32c4b-214">size</span><span class="sxs-lookup"><span data-stu-id="32c4b-214">size</span></span>|<span data-ttu-id="32c4b-215">Int64</span><span class="sxs-lookup"><span data-stu-id="32c4b-215">Int64</span></span>|<span data-ttu-id="32c4b-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="32c4b-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="32c4b-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="32c4b-218">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="32c4b-218">installCommandLine</span></span>|<span data-ttu-id="32c4b-219">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-219">String</span></span>|<span data-ttu-id="32c4b-220">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="32c4b-220">The command line to install this app</span></span>|
|<span data-ttu-id="32c4b-221">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="32c4b-221">uninstallCommandLine</span></span>|<span data-ttu-id="32c4b-222">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-222">String</span></span>|<span data-ttu-id="32c4b-223">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="32c4b-223">The command line to uninstall this app</span></span>|
|<span data-ttu-id="32c4b-224">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="32c4b-224">applicableArchitectures</span></span>|[<span data-ttu-id="32c4b-225">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="32c4b-225">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="32c4b-226">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="32c4b-226">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="32c4b-227">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="32c4b-227">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="32c4b-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="32c4b-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="32c4b-229">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="32c4b-229">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="32c4b-230">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="32c4b-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="32c4b-231">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="32c4b-231">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="32c4b-232">Int32</span><span class="sxs-lookup"><span data-stu-id="32c4b-232">Int32</span></span>|<span data-ttu-id="32c4b-233">O valor para o espaço livre mínimo em disco necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-233">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="32c4b-234">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="32c4b-234">minimumMemoryInMB</span></span>|<span data-ttu-id="32c4b-235">Int32</span><span class="sxs-lookup"><span data-stu-id="32c4b-235">Int32</span></span>|<span data-ttu-id="32c4b-236">O valor da memória física mínima exigida para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-236">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="32c4b-237">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="32c4b-237">minimumNumberOfProcessors</span></span>|<span data-ttu-id="32c4b-238">Int32</span><span class="sxs-lookup"><span data-stu-id="32c4b-238">Int32</span></span>|<span data-ttu-id="32c4b-239">O valor para o número mínimo de processadores necessários para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-239">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="32c4b-240">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="32c4b-240">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="32c4b-241">Int32</span><span class="sxs-lookup"><span data-stu-id="32c4b-241">Int32</span></span>|<span data-ttu-id="32c4b-242">O valor para a velocidade de CPU mínima necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-242">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="32c4b-243">detectionRules</span><span class="sxs-lookup"><span data-stu-id="32c4b-243">detectionRules</span></span>|<span data-ttu-id="32c4b-244">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="32c4b-245">As regras de detecção para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="32c4b-245">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="32c4b-246">requirementRules</span><span class="sxs-lookup"><span data-stu-id="32c4b-246">requirementRules</span></span>|<span data-ttu-id="32c4b-247">coleção [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="32c4b-248">As regras de requisito para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="32c4b-248">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="32c4b-249">installExperience</span><span class="sxs-lookup"><span data-stu-id="32c4b-249">installExperience</span></span>|[<span data-ttu-id="32c4b-250">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="32c4b-250">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="32c4b-251">A experiência de instalação para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32c4b-251">The install experience for this app.</span></span>|
|<span data-ttu-id="32c4b-252">returnCodes</span><span class="sxs-lookup"><span data-stu-id="32c4b-252">returnCodes</span></span>|<span data-ttu-id="32c4b-253">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="32c4b-253">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="32c4b-254">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="32c4b-254">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="32c4b-255">msiInformation</span><span class="sxs-lookup"><span data-stu-id="32c4b-255">msiInformation</span></span>|[<span data-ttu-id="32c4b-256">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="32c4b-256">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="32c4b-257">Os detalhes do MSI, se este aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="32c4b-257">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="32c4b-258">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="32c4b-258">setupFilePath</span></span>|<span data-ttu-id="32c4b-259">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-259">String</span></span>|<span data-ttu-id="32c4b-260">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="32c4b-260">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="32c4b-261">installLanguage</span><span class="sxs-lookup"><span data-stu-id="32c4b-261">installLanguage</span></span>|<span data-ttu-id="32c4b-262">String</span><span class="sxs-lookup"><span data-stu-id="32c4b-262">String</span></span>|<span data-ttu-id="32c4b-263">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="32c4b-263">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="32c4b-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="32c4b-264">Response</span></span>
<span data-ttu-id="32c4b-265">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32c4b-265">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32c4b-266">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32c4b-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="32c4b-267">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32c4b-267">Request</span></span>
<span data-ttu-id="32c4b-268">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32c4b-268">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2865

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```

### <a name="response"></a><span data-ttu-id="32c4b-269">Resposta</span><span class="sxs-lookup"><span data-stu-id="32c4b-269">Response</span></span>
<span data-ttu-id="32c4b-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32c4b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3037

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```





