---
title: Atualizar iosLobApp
description: Atualiza as propriedades de um objeto iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91cadd407a566545c16380187095634ccd52e9b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417134"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="8c482-103">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="8c482-103">Update iosLobApp</span></span>

<span data-ttu-id="8c482-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c482-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c482-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c482-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c482-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c482-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c482-107">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c482-107">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c482-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c482-108">Prerequisites</span></span>
<span data-ttu-id="8c482-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c482-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c482-111">Permission type</span></span>|<span data-ttu-id="8c482-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c482-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c482-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c482-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c482-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c482-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c482-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c482-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c482-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c482-116">Not supported.</span></span>|
|<span data-ttu-id="8c482-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c482-117">Application</span></span>|<span data-ttu-id="8c482-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c482-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c482-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c482-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8c482-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c482-120">Request headers</span></span>
|<span data-ttu-id="8c482-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c482-121">Header</span></span>|<span data-ttu-id="8c482-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c482-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c482-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c482-123">Authorization</span></span>|<span data-ttu-id="8c482-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c482-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c482-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c482-125">Accept</span></span>|<span data-ttu-id="8c482-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c482-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c482-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c482-127">Request body</span></span>
<span data-ttu-id="8c482-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c482-128">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="8c482-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune-apps-ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-129">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="8c482-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c482-130">Property</span></span>|<span data-ttu-id="8c482-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c482-131">Type</span></span>|<span data-ttu-id="8c482-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c482-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c482-133">id</span><span class="sxs-lookup"><span data-stu-id="8c482-133">id</span></span>|<span data-ttu-id="8c482-134">String</span><span class="sxs-lookup"><span data-stu-id="8c482-134">String</span></span>|<span data-ttu-id="8c482-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c482-135">Key of the entity.</span></span> <span data-ttu-id="8c482-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8c482-137">displayName</span></span>|<span data-ttu-id="8c482-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c482-138">String</span></span>|<span data-ttu-id="8c482-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8c482-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8c482-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-141">description</span><span class="sxs-lookup"><span data-stu-id="8c482-141">description</span></span>|<span data-ttu-id="8c482-142">String</span><span class="sxs-lookup"><span data-stu-id="8c482-142">String</span></span>|<span data-ttu-id="8c482-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c482-143">The description of the app.</span></span> <span data-ttu-id="8c482-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-145">publicador</span><span class="sxs-lookup"><span data-stu-id="8c482-145">publisher</span></span>|<span data-ttu-id="8c482-146">String</span><span class="sxs-lookup"><span data-stu-id="8c482-146">String</span></span>|<span data-ttu-id="8c482-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c482-147">The publisher of the app.</span></span> <span data-ttu-id="8c482-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8c482-149">largeIcon</span></span>|[<span data-ttu-id="8c482-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8c482-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8c482-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8c482-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8c482-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c482-153">createdDateTime</span></span>|<span data-ttu-id="8c482-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c482-154">DateTimeOffset</span></span>|<span data-ttu-id="8c482-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c482-155">The date and time the app was created.</span></span> <span data-ttu-id="8c482-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c482-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8c482-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c482-158">DateTimeOffset</span></span>|<span data-ttu-id="8c482-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8c482-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8c482-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8c482-161">isFeatured</span></span>|<span data-ttu-id="8c482-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c482-162">Boolean</span></span>|<span data-ttu-id="8c482-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8c482-164">privacyInformationUrl</span></span>|<span data-ttu-id="8c482-165">String</span><span class="sxs-lookup"><span data-stu-id="8c482-165">String</span></span>|<span data-ttu-id="8c482-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8c482-166">The privacy statement Url.</span></span> <span data-ttu-id="8c482-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8c482-168">informationUrl</span></span>|<span data-ttu-id="8c482-169">String</span><span class="sxs-lookup"><span data-stu-id="8c482-169">String</span></span>|<span data-ttu-id="8c482-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8c482-170">The more information Url.</span></span> <span data-ttu-id="8c482-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-172">owner</span><span class="sxs-lookup"><span data-stu-id="8c482-172">owner</span></span>|<span data-ttu-id="8c482-173">String</span><span class="sxs-lookup"><span data-stu-id="8c482-173">String</span></span>|<span data-ttu-id="8c482-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8c482-174">The owner of the app.</span></span> <span data-ttu-id="8c482-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-176">developer</span><span class="sxs-lookup"><span data-stu-id="8c482-176">developer</span></span>|<span data-ttu-id="8c482-177">String</span><span class="sxs-lookup"><span data-stu-id="8c482-177">String</span></span>|<span data-ttu-id="8c482-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c482-178">The developer of the app.</span></span> <span data-ttu-id="8c482-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-180">notes</span><span class="sxs-lookup"><span data-stu-id="8c482-180">notes</span></span>|<span data-ttu-id="8c482-181">String</span><span class="sxs-lookup"><span data-stu-id="8c482-181">String</span></span>|<span data-ttu-id="8c482-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c482-182">Notes for the app.</span></span> <span data-ttu-id="8c482-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8c482-184">uploadState</span></span>|<span data-ttu-id="8c482-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8c482-185">Int32</span></span>|<span data-ttu-id="8c482-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="8c482-186">The upload state.</span></span> <span data-ttu-id="8c482-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8c482-188">publishingState</span></span>|[<span data-ttu-id="8c482-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8c482-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8c482-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c482-190">The publishing state for the app.</span></span> <span data-ttu-id="8c482-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8c482-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8c482-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c482-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8c482-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8c482-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8c482-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8c482-194">isAssigned</span></span>|<span data-ttu-id="8c482-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c482-195">Boolean</span></span>|<span data-ttu-id="8c482-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="8c482-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8c482-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8c482-198">roleScopeTagIds</span></span>|<span data-ttu-id="8c482-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="8c482-199">String collection</span></span>|<span data-ttu-id="8c482-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8c482-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8c482-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8c482-202">dependentAppCount</span></span>|<span data-ttu-id="8c482-203">Int32</span><span class="sxs-lookup"><span data-stu-id="8c482-203">Int32</span></span>|<span data-ttu-id="8c482-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="8c482-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8c482-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c482-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8c482-206">committedContentVersion</span></span>|<span data-ttu-id="8c482-207">String</span><span class="sxs-lookup"><span data-stu-id="8c482-207">String</span></span>|<span data-ttu-id="8c482-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="8c482-208">The internal committed content version.</span></span> <span data-ttu-id="8c482-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8c482-210">fileName</span><span class="sxs-lookup"><span data-stu-id="8c482-210">fileName</span></span>|<span data-ttu-id="8c482-211">String</span><span class="sxs-lookup"><span data-stu-id="8c482-211">String</span></span>|<span data-ttu-id="8c482-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="8c482-212">The name of the main Lob application file.</span></span> <span data-ttu-id="8c482-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8c482-214">size</span><span class="sxs-lookup"><span data-stu-id="8c482-214">size</span></span>|<span data-ttu-id="8c482-215">Int64</span><span class="sxs-lookup"><span data-stu-id="8c482-215">Int64</span></span>|<span data-ttu-id="8c482-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="8c482-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="8c482-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c482-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8c482-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="8c482-218">bundleId</span></span>|<span data-ttu-id="8c482-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c482-219">String</span></span>|<span data-ttu-id="8c482-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8c482-220">The Identity Name.</span></span>|
|<span data-ttu-id="8c482-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="8c482-221">applicableDeviceType</span></span>|[<span data-ttu-id="8c482-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8c482-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="8c482-223">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="8c482-223">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="8c482-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8c482-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8c482-225">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8c482-225">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="8c482-226">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8c482-226">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8c482-227">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8c482-227">expirationDateTime</span></span>|<span data-ttu-id="8c482-228">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c482-228">DateTimeOffset</span></span>|<span data-ttu-id="8c482-229">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="8c482-229">The expiration time.</span></span>|
|<span data-ttu-id="8c482-230">versionNumber</span><span class="sxs-lookup"><span data-stu-id="8c482-230">versionNumber</span></span>|<span data-ttu-id="8c482-231">String</span><span class="sxs-lookup"><span data-stu-id="8c482-231">String</span></span>|<span data-ttu-id="8c482-232">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="8c482-232">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8c482-233">buildNumber</span><span class="sxs-lookup"><span data-stu-id="8c482-233">buildNumber</span></span>|<span data-ttu-id="8c482-234">String</span><span class="sxs-lookup"><span data-stu-id="8c482-234">String</span></span>|<span data-ttu-id="8c482-235">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="8c482-235">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8c482-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8c482-236">identityVersion</span></span>|<span data-ttu-id="8c482-237">String</span><span class="sxs-lookup"><span data-stu-id="8c482-237">String</span></span>|<span data-ttu-id="8c482-238">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="8c482-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="8c482-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c482-239">Response</span></span>
<span data-ttu-id="8c482-240">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c482-240">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c482-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c482-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c482-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c482-242">Request</span></span>
<span data-ttu-id="8c482-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c482-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1411

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="8c482-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c482-244">Response</span></span>
<span data-ttu-id="8c482-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c482-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1583

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```



