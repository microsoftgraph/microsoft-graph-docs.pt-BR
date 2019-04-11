---
title: Atualizar iosLobApp
description: Atualiza as propriedades de um objeto iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88e80c1aa29434d8cc7fad1319dca2f8da4d9f79
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780165"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="5ed11-103">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="5ed11-103">Update iosLobApp</span></span>

> <span data-ttu-id="5ed11-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ed11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ed11-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ed11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ed11-106">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5ed11-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ed11-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ed11-107">Prerequisites</span></span>
<span data-ttu-id="5ed11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ed11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ed11-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ed11-110">Permission type</span></span>|<span data-ttu-id="5ed11-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ed11-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ed11-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ed11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ed11-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ed11-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5ed11-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ed11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ed11-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ed11-115">Not supported.</span></span>|
|<span data-ttu-id="5ed11-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ed11-116">Application</span></span>|<span data-ttu-id="5ed11-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ed11-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ed11-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ed11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5ed11-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed11-119">Request headers</span></span>
|<span data-ttu-id="5ed11-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ed11-120">Header</span></span>|<span data-ttu-id="5ed11-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ed11-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ed11-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ed11-122">Authorization</span></span>|<span data-ttu-id="5ed11-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ed11-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ed11-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ed11-124">Accept</span></span>|<span data-ttu-id="5ed11-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ed11-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ed11-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed11-126">Request body</span></span>
<span data-ttu-id="5ed11-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5ed11-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="5ed11-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune-apps-ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="5ed11-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ed11-129">Property</span></span>|<span data-ttu-id="5ed11-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ed11-130">Type</span></span>|<span data-ttu-id="5ed11-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ed11-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed11-132">id</span><span class="sxs-lookup"><span data-stu-id="5ed11-132">id</span></span>|<span data-ttu-id="5ed11-133">String</span><span class="sxs-lookup"><span data-stu-id="5ed11-133">String</span></span>|<span data-ttu-id="5ed11-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ed11-134">Key of the entity.</span></span> <span data-ttu-id="5ed11-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5ed11-136">displayName</span></span>|<span data-ttu-id="5ed11-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-137">String</span></span>|<span data-ttu-id="5ed11-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="5ed11-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5ed11-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-140">description</span><span class="sxs-lookup"><span data-stu-id="5ed11-140">description</span></span>|<span data-ttu-id="5ed11-141">String</span><span class="sxs-lookup"><span data-stu-id="5ed11-141">String</span></span>|<span data-ttu-id="5ed11-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ed11-142">The description of the app.</span></span> <span data-ttu-id="5ed11-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-144">publicador</span><span class="sxs-lookup"><span data-stu-id="5ed11-144">publisher</span></span>|<span data-ttu-id="5ed11-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-145">String</span></span>|<span data-ttu-id="5ed11-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ed11-146">The publisher of the app.</span></span> <span data-ttu-id="5ed11-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5ed11-148">largeIcon</span></span>|[<span data-ttu-id="5ed11-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5ed11-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5ed11-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="5ed11-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5ed11-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed11-152">createdDateTime</span></span>|<span data-ttu-id="5ed11-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed11-153">DateTimeOffset</span></span>|<span data-ttu-id="5ed11-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ed11-154">The date and time the app was created.</span></span> <span data-ttu-id="5ed11-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed11-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5ed11-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed11-157">DateTimeOffset</span></span>|<span data-ttu-id="5ed11-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5ed11-158">The date and time the app was last modified.</span></span> <span data-ttu-id="5ed11-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5ed11-160">isFeatured</span></span>|<span data-ttu-id="5ed11-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ed11-161">Boolean</span></span>|<span data-ttu-id="5ed11-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5ed11-163">privacyInformationUrl</span></span>|<span data-ttu-id="5ed11-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-164">String</span></span>|<span data-ttu-id="5ed11-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5ed11-165">The privacy statement Url.</span></span> <span data-ttu-id="5ed11-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5ed11-167">informationUrl</span></span>|<span data-ttu-id="5ed11-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-168">String</span></span>|<span data-ttu-id="5ed11-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5ed11-169">The more information Url.</span></span> <span data-ttu-id="5ed11-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-171">owner</span><span class="sxs-lookup"><span data-stu-id="5ed11-171">owner</span></span>|<span data-ttu-id="5ed11-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-172">String</span></span>|<span data-ttu-id="5ed11-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5ed11-173">The owner of the app.</span></span> <span data-ttu-id="5ed11-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-175">developer</span><span class="sxs-lookup"><span data-stu-id="5ed11-175">developer</span></span>|<span data-ttu-id="5ed11-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-176">String</span></span>|<span data-ttu-id="5ed11-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ed11-177">The developer of the app.</span></span> <span data-ttu-id="5ed11-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-179">notes</span><span class="sxs-lookup"><span data-stu-id="5ed11-179">notes</span></span>|<span data-ttu-id="5ed11-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-180">String</span></span>|<span data-ttu-id="5ed11-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ed11-181">Notes for the app.</span></span> <span data-ttu-id="5ed11-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="5ed11-183">uploadState</span></span>|<span data-ttu-id="5ed11-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed11-184">Int32</span></span>|<span data-ttu-id="5ed11-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="5ed11-185">The upload state.</span></span> <span data-ttu-id="5ed11-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="5ed11-187">publishingState</span></span>|[<span data-ttu-id="5ed11-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5ed11-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5ed11-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ed11-189">The publishing state for the app.</span></span> <span data-ttu-id="5ed11-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="5ed11-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5ed11-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5ed11-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5ed11-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5ed11-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5ed11-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5ed11-193">isAssigned</span></span>|<span data-ttu-id="5ed11-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ed11-194">Boolean</span></span>|<span data-ttu-id="5ed11-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="5ed11-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5ed11-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ed11-197">roleScopeTagIds</span></span>|<span data-ttu-id="5ed11-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5ed11-198">String collection</span></span>|<span data-ttu-id="5ed11-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="5ed11-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5ed11-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="5ed11-201">dependentAppCount</span></span>|<span data-ttu-id="5ed11-202">Int32</span><span class="sxs-lookup"><span data-stu-id="5ed11-202">Int32</span></span>|<span data-ttu-id="5ed11-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="5ed11-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5ed11-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ed11-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5ed11-205">committedContentVersion</span></span>|<span data-ttu-id="5ed11-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-206">String</span></span>|<span data-ttu-id="5ed11-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="5ed11-207">The internal committed content version.</span></span> <span data-ttu-id="5ed11-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5ed11-209">fileName</span><span class="sxs-lookup"><span data-stu-id="5ed11-209">fileName</span></span>|<span data-ttu-id="5ed11-210">String</span><span class="sxs-lookup"><span data-stu-id="5ed11-210">String</span></span>|<span data-ttu-id="5ed11-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="5ed11-211">The name of the main Lob application file.</span></span> <span data-ttu-id="5ed11-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5ed11-213">size</span><span class="sxs-lookup"><span data-stu-id="5ed11-213">size</span></span>|<span data-ttu-id="5ed11-214">Int64</span><span class="sxs-lookup"><span data-stu-id="5ed11-214">Int64</span></span>|<span data-ttu-id="5ed11-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="5ed11-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="5ed11-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed11-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5ed11-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="5ed11-217">bundleId</span></span>|<span data-ttu-id="5ed11-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-218">String</span></span>|<span data-ttu-id="5ed11-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="5ed11-219">The Identity Name.</span></span>|
|<span data-ttu-id="5ed11-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5ed11-220">applicableDeviceType</span></span>|[<span data-ttu-id="5ed11-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5ed11-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5ed11-222">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="5ed11-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5ed11-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5ed11-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5ed11-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5ed11-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="5ed11-225">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="5ed11-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5ed11-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed11-226">expirationDateTime</span></span>|<span data-ttu-id="5ed11-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed11-227">DateTimeOffset</span></span>|<span data-ttu-id="5ed11-228">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="5ed11-228">The expiration time.</span></span>|
|<span data-ttu-id="5ed11-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="5ed11-229">versionNumber</span></span>|<span data-ttu-id="5ed11-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-230">String</span></span>|<span data-ttu-id="5ed11-231">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="5ed11-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5ed11-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="5ed11-232">buildNumber</span></span>|<span data-ttu-id="5ed11-233">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed11-233">String</span></span>|<span data-ttu-id="5ed11-234">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="5ed11-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5ed11-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5ed11-235">identityVersion</span></span>|<span data-ttu-id="5ed11-236">String</span><span class="sxs-lookup"><span data-stu-id="5ed11-236">String</span></span>|<span data-ttu-id="5ed11-237">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="5ed11-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="5ed11-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ed11-238">Response</span></span>
<span data-ttu-id="5ed11-239">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ed11-239">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ed11-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ed11-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ed11-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed11-241">Request</span></span>
<span data-ttu-id="5ed11-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ed11-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1391

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="5ed11-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ed11-243">Response</span></span>
<span data-ttu-id="5ed11-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ed11-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1563

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





