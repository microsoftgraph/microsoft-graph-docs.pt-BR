---
title: Atualizar macOSLobApp
description: Atualiza as propriedades de um objeto macOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c67231a85de9be6aff0e8d997cac4a0b3a8eaed
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535349"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="d066b-103">Atualizar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="d066b-103">Update macOSLobApp</span></span>

> <span data-ttu-id="d066b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d066b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d066b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d066b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d066b-106">Atualiza as propriedades de um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d066b-106">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d066b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d066b-107">Prerequisites</span></span>
<span data-ttu-id="d066b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d066b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d066b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d066b-110">Permission type</span></span>|<span data-ttu-id="d066b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d066b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d066b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d066b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d066b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d066b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d066b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d066b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d066b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d066b-115">Not supported.</span></span>|
|<span data-ttu-id="d066b-116">Application</span><span class="sxs-lookup"><span data-stu-id="d066b-116">Application</span></span>|<span data-ttu-id="d066b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d066b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d066b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d066b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d066b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d066b-119">Request headers</span></span>
|<span data-ttu-id="d066b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d066b-120">Header</span></span>|<span data-ttu-id="d066b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d066b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d066b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d066b-122">Authorization</span></span>|<span data-ttu-id="d066b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d066b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d066b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d066b-124">Accept</span></span>|<span data-ttu-id="d066b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d066b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d066b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d066b-126">Request body</span></span>
<span data-ttu-id="d066b-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d066b-127">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="d066b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d066b-128">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="d066b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d066b-129">Property</span></span>|<span data-ttu-id="d066b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d066b-130">Type</span></span>|<span data-ttu-id="d066b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d066b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d066b-132">id</span><span class="sxs-lookup"><span data-stu-id="d066b-132">id</span></span>|<span data-ttu-id="d066b-133">String</span><span class="sxs-lookup"><span data-stu-id="d066b-133">String</span></span>|<span data-ttu-id="d066b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d066b-134">Key of the entity.</span></span> <span data-ttu-id="d066b-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d066b-136">displayName</span></span>|<span data-ttu-id="d066b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-137">String</span></span>|<span data-ttu-id="d066b-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d066b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d066b-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-140">description</span><span class="sxs-lookup"><span data-stu-id="d066b-140">description</span></span>|<span data-ttu-id="d066b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-141">String</span></span>|<span data-ttu-id="d066b-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d066b-142">The description of the app.</span></span> <span data-ttu-id="d066b-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-144">publicador</span><span class="sxs-lookup"><span data-stu-id="d066b-144">publisher</span></span>|<span data-ttu-id="d066b-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-145">String</span></span>|<span data-ttu-id="d066b-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d066b-146">The publisher of the app.</span></span> <span data-ttu-id="d066b-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d066b-148">largeIcon</span></span>|[<span data-ttu-id="d066b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d066b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d066b-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d066b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d066b-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d066b-152">createdDateTime</span></span>|<span data-ttu-id="d066b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d066b-153">DateTimeOffset</span></span>|<span data-ttu-id="d066b-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d066b-154">The date and time the app was created.</span></span> <span data-ttu-id="d066b-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d066b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d066b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d066b-157">DateTimeOffset</span></span>|<span data-ttu-id="d066b-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d066b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d066b-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d066b-160">isFeatured</span></span>|<span data-ttu-id="d066b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d066b-161">Boolean</span></span>|<span data-ttu-id="d066b-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d066b-163">privacyInformationUrl</span></span>|<span data-ttu-id="d066b-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-164">String</span></span>|<span data-ttu-id="d066b-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d066b-165">The privacy statement Url.</span></span> <span data-ttu-id="d066b-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d066b-167">informationUrl</span></span>|<span data-ttu-id="d066b-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-168">String</span></span>|<span data-ttu-id="d066b-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d066b-169">The more information Url.</span></span> <span data-ttu-id="d066b-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-171">owner</span><span class="sxs-lookup"><span data-stu-id="d066b-171">owner</span></span>|<span data-ttu-id="d066b-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-172">String</span></span>|<span data-ttu-id="d066b-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d066b-173">The owner of the app.</span></span> <span data-ttu-id="d066b-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-175">developer</span><span class="sxs-lookup"><span data-stu-id="d066b-175">developer</span></span>|<span data-ttu-id="d066b-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-176">String</span></span>|<span data-ttu-id="d066b-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d066b-177">The developer of the app.</span></span> <span data-ttu-id="d066b-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-179">notes</span><span class="sxs-lookup"><span data-stu-id="d066b-179">notes</span></span>|<span data-ttu-id="d066b-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-180">String</span></span>|<span data-ttu-id="d066b-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d066b-181">Notes for the app.</span></span> <span data-ttu-id="d066b-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d066b-183">uploadState</span></span>|<span data-ttu-id="d066b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d066b-184">Int32</span></span>|<span data-ttu-id="d066b-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="d066b-185">The upload state.</span></span> <span data-ttu-id="d066b-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d066b-187">publishingState</span></span>|[<span data-ttu-id="d066b-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d066b-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d066b-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d066b-189">The publishing state for the app.</span></span> <span data-ttu-id="d066b-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d066b-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d066b-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d066b-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d066b-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d066b-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d066b-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d066b-193">isAssigned</span></span>|<span data-ttu-id="d066b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d066b-194">Boolean</span></span>|<span data-ttu-id="d066b-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="d066b-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d066b-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d066b-197">roleScopeTagIds</span></span>|<span data-ttu-id="d066b-198">String collection</span><span class="sxs-lookup"><span data-stu-id="d066b-198">String collection</span></span>|<span data-ttu-id="d066b-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d066b-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d066b-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d066b-201">dependentAppCount</span></span>|<span data-ttu-id="d066b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d066b-202">Int32</span></span>|<span data-ttu-id="d066b-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="d066b-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d066b-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d066b-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d066b-205">committedContentVersion</span></span>|<span data-ttu-id="d066b-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-206">String</span></span>|<span data-ttu-id="d066b-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="d066b-207">The internal committed content version.</span></span> <span data-ttu-id="d066b-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d066b-209">fileName</span><span class="sxs-lookup"><span data-stu-id="d066b-209">fileName</span></span>|<span data-ttu-id="d066b-210">String</span><span class="sxs-lookup"><span data-stu-id="d066b-210">String</span></span>|<span data-ttu-id="d066b-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="d066b-211">The name of the main Lob application file.</span></span> <span data-ttu-id="d066b-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d066b-213">size</span><span class="sxs-lookup"><span data-stu-id="d066b-213">size</span></span>|<span data-ttu-id="d066b-214">Int64</span><span class="sxs-lookup"><span data-stu-id="d066b-214">Int64</span></span>|<span data-ttu-id="d066b-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="d066b-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="d066b-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d066b-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="d066b-217">bundleId</span></span>|<span data-ttu-id="d066b-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-218">String</span></span>|<span data-ttu-id="d066b-219">A ID do pacote.</span><span class="sxs-lookup"><span data-stu-id="d066b-219">The bundle id.</span></span>|
|<span data-ttu-id="d066b-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d066b-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d066b-221">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d066b-221">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="d066b-222">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="d066b-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d066b-223">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d066b-223">buildNumber</span></span>|<span data-ttu-id="d066b-224">String</span><span class="sxs-lookup"><span data-stu-id="d066b-224">String</span></span>|<span data-ttu-id="d066b-225">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="d066b-225">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d066b-226">versionNumber</span><span class="sxs-lookup"><span data-stu-id="d066b-226">versionNumber</span></span>|<span data-ttu-id="d066b-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d066b-227">String</span></span>|<span data-ttu-id="d066b-228">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="d066b-228">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d066b-229">childApps</span><span class="sxs-lookup"><span data-stu-id="d066b-229">childApps</span></span>|<span data-ttu-id="d066b-230">coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="d066b-230">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="d066b-231">A lista de aplicativos neste pacote de pacotes</span><span class="sxs-lookup"><span data-stu-id="d066b-231">The app list in this bundle package</span></span>|
|<span data-ttu-id="d066b-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d066b-232">identityVersion</span></span>|<span data-ttu-id="d066b-233">String</span><span class="sxs-lookup"><span data-stu-id="d066b-233">String</span></span>|<span data-ttu-id="d066b-234">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="d066b-234">The identity version.</span></span>|
|<span data-ttu-id="d066b-235">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="d066b-235">md5HashChunkSize</span></span>|<span data-ttu-id="d066b-236">Int32</span><span class="sxs-lookup"><span data-stu-id="d066b-236">Int32</span></span>|<span data-ttu-id="d066b-237">O tamanho da parte do hash MD5</span><span class="sxs-lookup"><span data-stu-id="d066b-237">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="d066b-238">md5Hash</span><span class="sxs-lookup"><span data-stu-id="d066b-238">md5Hash</span></span>|<span data-ttu-id="d066b-239">String collection</span><span class="sxs-lookup"><span data-stu-id="d066b-239">String collection</span></span>|<span data-ttu-id="d066b-240">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="d066b-240">The MD5 hash codes</span></span>|
|<span data-ttu-id="d066b-241">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="d066b-241">ignoreVersionDetection</span></span>|<span data-ttu-id="d066b-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="d066b-242">Boolean</span></span>|<span data-ttu-id="d066b-243">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d066b-243">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="d066b-244">Defina isso como true para aplicativos de linha de negócios (LoB) de macOS que usam um recurso de autoatualização.</span><span class="sxs-lookup"><span data-stu-id="d066b-244">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="d066b-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="d066b-245">Response</span></span>
<span data-ttu-id="d066b-246">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d066b-246">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d066b-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d066b-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="d066b-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d066b-248">Request</span></span>
<span data-ttu-id="d066b-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d066b-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="d066b-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="d066b-250">Response</span></span>
<span data-ttu-id="d066b-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d066b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






