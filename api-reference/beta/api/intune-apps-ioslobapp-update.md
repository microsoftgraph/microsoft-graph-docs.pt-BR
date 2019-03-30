---
title: Atualizar iosLobApp
description: Atualiza as propriedades de um objeto iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46d6aa0294375f0e2074b50dee45f2a5be267d75
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986499"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="3946d-103">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="3946d-103">Update iosLobApp</span></span>

> <span data-ttu-id="3946d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3946d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3946d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3946d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3946d-106">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3946d-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3946d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3946d-107">Prerequisites</span></span>
<span data-ttu-id="3946d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3946d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3946d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3946d-110">Permission type</span></span>|<span data-ttu-id="3946d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3946d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3946d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3946d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3946d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3946d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3946d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3946d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3946d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3946d-115">Not supported.</span></span>|
|<span data-ttu-id="3946d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3946d-116">Application</span></span>|<span data-ttu-id="3946d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3946d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3946d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3946d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3946d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3946d-119">Request headers</span></span>
|<span data-ttu-id="3946d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3946d-120">Header</span></span>|<span data-ttu-id="3946d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3946d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3946d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3946d-122">Authorization</span></span>|<span data-ttu-id="3946d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3946d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3946d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3946d-124">Accept</span></span>|<span data-ttu-id="3946d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3946d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3946d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3946d-126">Request body</span></span>
<span data-ttu-id="3946d-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3946d-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="3946d-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune-apps-ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="3946d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3946d-129">Property</span></span>|<span data-ttu-id="3946d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3946d-130">Type</span></span>|<span data-ttu-id="3946d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3946d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3946d-132">id</span><span class="sxs-lookup"><span data-stu-id="3946d-132">id</span></span>|<span data-ttu-id="3946d-133">String</span><span class="sxs-lookup"><span data-stu-id="3946d-133">String</span></span>|<span data-ttu-id="3946d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3946d-134">Key of the entity.</span></span> <span data-ttu-id="3946d-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3946d-136">displayName</span></span>|<span data-ttu-id="3946d-137">String</span><span class="sxs-lookup"><span data-stu-id="3946d-137">String</span></span>|<span data-ttu-id="3946d-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3946d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3946d-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-140">description</span><span class="sxs-lookup"><span data-stu-id="3946d-140">description</span></span>|<span data-ttu-id="3946d-141">String</span><span class="sxs-lookup"><span data-stu-id="3946d-141">String</span></span>|<span data-ttu-id="3946d-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3946d-142">The description of the app.</span></span> <span data-ttu-id="3946d-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-144">publicador</span><span class="sxs-lookup"><span data-stu-id="3946d-144">publisher</span></span>|<span data-ttu-id="3946d-145">String</span><span class="sxs-lookup"><span data-stu-id="3946d-145">String</span></span>|<span data-ttu-id="3946d-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3946d-146">The publisher of the app.</span></span> <span data-ttu-id="3946d-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3946d-148">largeIcon</span></span>|[<span data-ttu-id="3946d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3946d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3946d-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3946d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3946d-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3946d-152">createdDateTime</span></span>|<span data-ttu-id="3946d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3946d-153">DateTimeOffset</span></span>|<span data-ttu-id="3946d-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3946d-154">The date and time the app was created.</span></span> <span data-ttu-id="3946d-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3946d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3946d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3946d-157">DateTimeOffset</span></span>|<span data-ttu-id="3946d-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3946d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3946d-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3946d-160">isFeatured</span></span>|<span data-ttu-id="3946d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3946d-161">Boolean</span></span>|<span data-ttu-id="3946d-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3946d-163">privacyInformationUrl</span></span>|<span data-ttu-id="3946d-164">String</span><span class="sxs-lookup"><span data-stu-id="3946d-164">String</span></span>|<span data-ttu-id="3946d-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3946d-165">The privacy statement Url.</span></span> <span data-ttu-id="3946d-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3946d-167">informationUrl</span></span>|<span data-ttu-id="3946d-168">String</span><span class="sxs-lookup"><span data-stu-id="3946d-168">String</span></span>|<span data-ttu-id="3946d-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3946d-169">The more information Url.</span></span> <span data-ttu-id="3946d-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-171">owner</span><span class="sxs-lookup"><span data-stu-id="3946d-171">owner</span></span>|<span data-ttu-id="3946d-172">String</span><span class="sxs-lookup"><span data-stu-id="3946d-172">String</span></span>|<span data-ttu-id="3946d-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3946d-173">The owner of the app.</span></span> <span data-ttu-id="3946d-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-175">developer</span><span class="sxs-lookup"><span data-stu-id="3946d-175">developer</span></span>|<span data-ttu-id="3946d-176">String</span><span class="sxs-lookup"><span data-stu-id="3946d-176">String</span></span>|<span data-ttu-id="3946d-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3946d-177">The developer of the app.</span></span> <span data-ttu-id="3946d-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-179">notes</span><span class="sxs-lookup"><span data-stu-id="3946d-179">notes</span></span>|<span data-ttu-id="3946d-180">String</span><span class="sxs-lookup"><span data-stu-id="3946d-180">String</span></span>|<span data-ttu-id="3946d-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3946d-181">Notes for the app.</span></span> <span data-ttu-id="3946d-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3946d-183">uploadState</span></span>|<span data-ttu-id="3946d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3946d-184">Int32</span></span>|<span data-ttu-id="3946d-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="3946d-185">The upload state.</span></span> <span data-ttu-id="3946d-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3946d-187">publishingState</span></span>|[<span data-ttu-id="3946d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3946d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3946d-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3946d-189">The publishing state for the app.</span></span> <span data-ttu-id="3946d-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3946d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3946d-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3946d-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3946d-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3946d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3946d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3946d-193">isAssigned</span></span>|<span data-ttu-id="3946d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3946d-194">Boolean</span></span>|<span data-ttu-id="3946d-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="3946d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3946d-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3946d-197">roleScopeTagIds</span></span>|<span data-ttu-id="3946d-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="3946d-198">String collection</span></span>|<span data-ttu-id="3946d-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="3946d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3946d-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3946d-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3946d-201">committedContentVersion</span></span>|<span data-ttu-id="3946d-202">String</span><span class="sxs-lookup"><span data-stu-id="3946d-202">String</span></span>|<span data-ttu-id="3946d-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="3946d-203">The internal committed content version.</span></span> <span data-ttu-id="3946d-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3946d-205">fileName</span><span class="sxs-lookup"><span data-stu-id="3946d-205">fileName</span></span>|<span data-ttu-id="3946d-206">String</span><span class="sxs-lookup"><span data-stu-id="3946d-206">String</span></span>|<span data-ttu-id="3946d-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="3946d-207">The name of the main Lob application file.</span></span> <span data-ttu-id="3946d-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3946d-209">size</span><span class="sxs-lookup"><span data-stu-id="3946d-209">size</span></span>|<span data-ttu-id="3946d-210">Int64</span><span class="sxs-lookup"><span data-stu-id="3946d-210">Int64</span></span>|<span data-ttu-id="3946d-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="3946d-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="3946d-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3946d-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3946d-213">bundleId</span><span class="sxs-lookup"><span data-stu-id="3946d-213">bundleId</span></span>|<span data-ttu-id="3946d-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3946d-214">String</span></span>|<span data-ttu-id="3946d-215">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="3946d-215">The Identity Name.</span></span>|
|<span data-ttu-id="3946d-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3946d-216">applicableDeviceType</span></span>|[<span data-ttu-id="3946d-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3946d-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="3946d-218">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="3946d-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3946d-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3946d-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3946d-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3946d-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="3946d-221">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="3946d-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3946d-222">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3946d-222">expirationDateTime</span></span>|<span data-ttu-id="3946d-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3946d-223">DateTimeOffset</span></span>|<span data-ttu-id="3946d-224">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="3946d-224">The expiration time.</span></span>|
|<span data-ttu-id="3946d-225">versionNumber</span><span class="sxs-lookup"><span data-stu-id="3946d-225">versionNumber</span></span>|<span data-ttu-id="3946d-226">String</span><span class="sxs-lookup"><span data-stu-id="3946d-226">String</span></span>|<span data-ttu-id="3946d-227">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="3946d-227">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3946d-228">buildNumber</span><span class="sxs-lookup"><span data-stu-id="3946d-228">buildNumber</span></span>|<span data-ttu-id="3946d-229">String</span><span class="sxs-lookup"><span data-stu-id="3946d-229">String</span></span>|<span data-ttu-id="3946d-230">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="3946d-230">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3946d-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3946d-231">identityVersion</span></span>|<span data-ttu-id="3946d-232">String</span><span class="sxs-lookup"><span data-stu-id="3946d-232">String</span></span>|<span data-ttu-id="3946d-233">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="3946d-233">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="3946d-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="3946d-234">Response</span></span>
<span data-ttu-id="3946d-235">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3946d-235">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3946d-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3946d-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="3946d-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3946d-237">Request</span></span>
<span data-ttu-id="3946d-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3946d-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1364

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

### <a name="response"></a><span data-ttu-id="3946d-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="3946d-239">Response</span></span>
<span data-ttu-id="3946d-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3946d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1536

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




