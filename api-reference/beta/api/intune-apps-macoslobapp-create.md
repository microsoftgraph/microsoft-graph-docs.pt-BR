---
title: Criar macOSLobApp
description: Criar um novo objeto macOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d12b3519731f93f8eec561f0806770be079b87a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394367"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="b499c-103">Criar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="b499c-103">Create macOSLobApp</span></span>

<span data-ttu-id="b499c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b499c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b499c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b499c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b499c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b499c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b499c-107">Criar um novo objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b499c-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b499c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b499c-108">Prerequisites</span></span>
<span data-ttu-id="b499c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b499c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b499c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b499c-111">Permission type</span></span>|<span data-ttu-id="b499c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b499c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b499c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b499c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b499c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b499c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b499c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b499c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b499c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b499c-116">Not supported.</span></span>|
|<span data-ttu-id="b499c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b499c-117">Application</span></span>|<span data-ttu-id="b499c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b499c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b499c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b499c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b499c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b499c-120">Request headers</span></span>
|<span data-ttu-id="b499c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b499c-121">Header</span></span>|<span data-ttu-id="b499c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b499c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b499c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b499c-123">Authorization</span></span>|<span data-ttu-id="b499c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b499c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b499c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b499c-125">Accept</span></span>|<span data-ttu-id="b499c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b499c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b499c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b499c-127">Request body</span></span>
<span data-ttu-id="b499c-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="b499c-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="b499c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="b499c-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="b499c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b499c-130">Property</span></span>|<span data-ttu-id="b499c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b499c-131">Type</span></span>|<span data-ttu-id="b499c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b499c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b499c-133">id</span><span class="sxs-lookup"><span data-stu-id="b499c-133">id</span></span>|<span data-ttu-id="b499c-134">String</span><span class="sxs-lookup"><span data-stu-id="b499c-134">String</span></span>|<span data-ttu-id="b499c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b499c-135">Key of the entity.</span></span> <span data-ttu-id="b499c-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b499c-137">displayName</span></span>|<span data-ttu-id="b499c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b499c-138">String</span></span>|<span data-ttu-id="b499c-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b499c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b499c-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-141">description</span><span class="sxs-lookup"><span data-stu-id="b499c-141">description</span></span>|<span data-ttu-id="b499c-142">String</span><span class="sxs-lookup"><span data-stu-id="b499c-142">String</span></span>|<span data-ttu-id="b499c-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b499c-143">The description of the app.</span></span> <span data-ttu-id="b499c-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-145">publicador</span><span class="sxs-lookup"><span data-stu-id="b499c-145">publisher</span></span>|<span data-ttu-id="b499c-146">String</span><span class="sxs-lookup"><span data-stu-id="b499c-146">String</span></span>|<span data-ttu-id="b499c-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b499c-147">The publisher of the app.</span></span> <span data-ttu-id="b499c-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b499c-149">largeIcon</span></span>|[<span data-ttu-id="b499c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b499c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b499c-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b499c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b499c-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b499c-153">createdDateTime</span></span>|<span data-ttu-id="b499c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b499c-154">DateTimeOffset</span></span>|<span data-ttu-id="b499c-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b499c-155">The date and time the app was created.</span></span> <span data-ttu-id="b499c-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b499c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b499c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b499c-158">DateTimeOffset</span></span>|<span data-ttu-id="b499c-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b499c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b499c-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b499c-161">isFeatured</span></span>|<span data-ttu-id="b499c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b499c-162">Boolean</span></span>|<span data-ttu-id="b499c-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b499c-164">privacyInformationUrl</span></span>|<span data-ttu-id="b499c-165">String</span><span class="sxs-lookup"><span data-stu-id="b499c-165">String</span></span>|<span data-ttu-id="b499c-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b499c-166">The privacy statement Url.</span></span> <span data-ttu-id="b499c-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b499c-168">informationUrl</span></span>|<span data-ttu-id="b499c-169">String</span><span class="sxs-lookup"><span data-stu-id="b499c-169">String</span></span>|<span data-ttu-id="b499c-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b499c-170">The more information Url.</span></span> <span data-ttu-id="b499c-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-172">owner</span><span class="sxs-lookup"><span data-stu-id="b499c-172">owner</span></span>|<span data-ttu-id="b499c-173">String</span><span class="sxs-lookup"><span data-stu-id="b499c-173">String</span></span>|<span data-ttu-id="b499c-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b499c-174">The owner of the app.</span></span> <span data-ttu-id="b499c-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-176">developer</span><span class="sxs-lookup"><span data-stu-id="b499c-176">developer</span></span>|<span data-ttu-id="b499c-177">String</span><span class="sxs-lookup"><span data-stu-id="b499c-177">String</span></span>|<span data-ttu-id="b499c-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b499c-178">The developer of the app.</span></span> <span data-ttu-id="b499c-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-180">notes</span><span class="sxs-lookup"><span data-stu-id="b499c-180">notes</span></span>|<span data-ttu-id="b499c-181">String</span><span class="sxs-lookup"><span data-stu-id="b499c-181">String</span></span>|<span data-ttu-id="b499c-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b499c-182">Notes for the app.</span></span> <span data-ttu-id="b499c-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b499c-184">uploadState</span></span>|<span data-ttu-id="b499c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b499c-185">Int32</span></span>|<span data-ttu-id="b499c-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="b499c-186">The upload state.</span></span> <span data-ttu-id="b499c-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b499c-188">publishingState</span></span>|[<span data-ttu-id="b499c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b499c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b499c-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b499c-190">The publishing state for the app.</span></span> <span data-ttu-id="b499c-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b499c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b499c-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b499c-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b499c-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b499c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b499c-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b499c-194">isAssigned</span></span>|<span data-ttu-id="b499c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b499c-195">Boolean</span></span>|<span data-ttu-id="b499c-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="b499c-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b499c-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b499c-198">roleScopeTagIds</span></span>|<span data-ttu-id="b499c-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b499c-199">String collection</span></span>|<span data-ttu-id="b499c-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b499c-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b499c-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b499c-202">dependentAppCount</span></span>|<span data-ttu-id="b499c-203">Int32</span><span class="sxs-lookup"><span data-stu-id="b499c-203">Int32</span></span>|<span data-ttu-id="b499c-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="b499c-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b499c-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b499c-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b499c-206">committedContentVersion</span></span>|<span data-ttu-id="b499c-207">String</span><span class="sxs-lookup"><span data-stu-id="b499c-207">String</span></span>|<span data-ttu-id="b499c-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="b499c-208">The internal committed content version.</span></span> <span data-ttu-id="b499c-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b499c-210">fileName</span><span class="sxs-lookup"><span data-stu-id="b499c-210">fileName</span></span>|<span data-ttu-id="b499c-211">String</span><span class="sxs-lookup"><span data-stu-id="b499c-211">String</span></span>|<span data-ttu-id="b499c-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="b499c-212">The name of the main Lob application file.</span></span> <span data-ttu-id="b499c-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b499c-214">size</span><span class="sxs-lookup"><span data-stu-id="b499c-214">size</span></span>|<span data-ttu-id="b499c-215">Int64</span><span class="sxs-lookup"><span data-stu-id="b499c-215">Int64</span></span>|<span data-ttu-id="b499c-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="b499c-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="b499c-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b499c-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="b499c-218">bundleId</span></span>|<span data-ttu-id="b499c-219">String</span><span class="sxs-lookup"><span data-stu-id="b499c-219">String</span></span>|<span data-ttu-id="b499c-220">A ID do pacote.</span><span class="sxs-lookup"><span data-stu-id="b499c-220">The bundle id.</span></span>|
|<span data-ttu-id="b499c-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b499c-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b499c-222">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b499c-222">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="b499c-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b499c-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b499c-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="b499c-224">buildNumber</span></span>|<span data-ttu-id="b499c-225">String</span><span class="sxs-lookup"><span data-stu-id="b499c-225">String</span></span>|<span data-ttu-id="b499c-226">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="b499c-226">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b499c-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="b499c-227">versionNumber</span></span>|<span data-ttu-id="b499c-228">String</span><span class="sxs-lookup"><span data-stu-id="b499c-228">String</span></span>|<span data-ttu-id="b499c-229">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="b499c-229">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b499c-230">childApps</span><span class="sxs-lookup"><span data-stu-id="b499c-230">childApps</span></span>|<span data-ttu-id="b499c-231">coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="b499c-231">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="b499c-232">A lista de aplicativos neste pacote de pacotes</span><span class="sxs-lookup"><span data-stu-id="b499c-232">The app list in this bundle package</span></span>|
|<span data-ttu-id="b499c-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b499c-233">identityVersion</span></span>|<span data-ttu-id="b499c-234">String</span><span class="sxs-lookup"><span data-stu-id="b499c-234">String</span></span>|<span data-ttu-id="b499c-235">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="b499c-235">The identity version.</span></span>|
|<span data-ttu-id="b499c-236">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="b499c-236">md5HashChunkSize</span></span>|<span data-ttu-id="b499c-237">Int32</span><span class="sxs-lookup"><span data-stu-id="b499c-237">Int32</span></span>|<span data-ttu-id="b499c-238">O tamanho da parte do hash MD5</span><span class="sxs-lookup"><span data-stu-id="b499c-238">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="b499c-239">md5Hash</span><span class="sxs-lookup"><span data-stu-id="b499c-239">md5Hash</span></span>|<span data-ttu-id="b499c-240">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b499c-240">String collection</span></span>|<span data-ttu-id="b499c-241">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="b499c-241">The MD5 hash codes</span></span>|
|<span data-ttu-id="b499c-242">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="b499c-242">ignoreVersionDetection</span></span>|<span data-ttu-id="b499c-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="b499c-243">Boolean</span></span>|<span data-ttu-id="b499c-244">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b499c-244">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="b499c-245">Defina isso como true para aplicativos de linha de negócios (LoB) de macOS que usam um recurso de autoatualização.</span><span class="sxs-lookup"><span data-stu-id="b499c-245">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="b499c-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="b499c-246">Response</span></span>
<span data-ttu-id="b499c-247">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b499c-247">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b499c-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b499c-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="b499c-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b499c-249">Request</span></span>
<span data-ttu-id="b499c-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b499c-250">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b499c-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="b499c-251">Response</span></span>
<span data-ttu-id="b499c-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b499c-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



