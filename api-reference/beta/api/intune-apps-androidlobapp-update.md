---
title: Atualizar androidLobApp
description: Atualiza as propriedades de um objeto androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f2cc9177d374e7720821b9195a8b4d40bf2cf55
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784597"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="397c2-103">Atualizar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="397c2-103">Update androidLobApp</span></span>

> <span data-ttu-id="397c2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="397c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="397c2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="397c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="397c2-106">Atualiza as propriedades de um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="397c2-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="397c2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="397c2-107">Prerequisites</span></span>
<span data-ttu-id="397c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="397c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="397c2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="397c2-110">Permission type</span></span>|<span data-ttu-id="397c2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="397c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="397c2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="397c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="397c2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="397c2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="397c2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="397c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="397c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="397c2-115">Not supported.</span></span>|
|<span data-ttu-id="397c2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="397c2-116">Application</span></span>|<span data-ttu-id="397c2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="397c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="397c2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="397c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="397c2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="397c2-119">Request headers</span></span>
|<span data-ttu-id="397c2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="397c2-120">Header</span></span>|<span data-ttu-id="397c2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="397c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="397c2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="397c2-122">Authorization</span></span>|<span data-ttu-id="397c2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="397c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="397c2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="397c2-124">Accept</span></span>|<span data-ttu-id="397c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="397c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="397c2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="397c2-126">Request body</span></span>
<span data-ttu-id="397c2-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="397c2-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="397c2-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="397c2-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="397c2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="397c2-129">Property</span></span>|<span data-ttu-id="397c2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="397c2-130">Type</span></span>|<span data-ttu-id="397c2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="397c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="397c2-132">id</span><span class="sxs-lookup"><span data-stu-id="397c2-132">id</span></span>|<span data-ttu-id="397c2-133">String</span><span class="sxs-lookup"><span data-stu-id="397c2-133">String</span></span>|<span data-ttu-id="397c2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="397c2-134">Key of the entity.</span></span> <span data-ttu-id="397c2-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="397c2-136">displayName</span></span>|<span data-ttu-id="397c2-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-137">String</span></span>|<span data-ttu-id="397c2-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="397c2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="397c2-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-140">description</span><span class="sxs-lookup"><span data-stu-id="397c2-140">description</span></span>|<span data-ttu-id="397c2-141">String</span><span class="sxs-lookup"><span data-stu-id="397c2-141">String</span></span>|<span data-ttu-id="397c2-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="397c2-142">The description of the app.</span></span> <span data-ttu-id="397c2-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-144">publicador</span><span class="sxs-lookup"><span data-stu-id="397c2-144">publisher</span></span>|<span data-ttu-id="397c2-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-145">String</span></span>|<span data-ttu-id="397c2-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="397c2-146">The publisher of the app.</span></span> <span data-ttu-id="397c2-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="397c2-148">largeIcon</span></span>|[<span data-ttu-id="397c2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="397c2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="397c2-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="397c2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="397c2-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="397c2-152">createdDateTime</span></span>|<span data-ttu-id="397c2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="397c2-153">DateTimeOffset</span></span>|<span data-ttu-id="397c2-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="397c2-154">The date and time the app was created.</span></span> <span data-ttu-id="397c2-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="397c2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="397c2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="397c2-157">DateTimeOffset</span></span>|<span data-ttu-id="397c2-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="397c2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="397c2-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="397c2-160">isFeatured</span></span>|<span data-ttu-id="397c2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="397c2-161">Boolean</span></span>|<span data-ttu-id="397c2-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="397c2-163">privacyInformationUrl</span></span>|<span data-ttu-id="397c2-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-164">String</span></span>|<span data-ttu-id="397c2-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="397c2-165">The privacy statement Url.</span></span> <span data-ttu-id="397c2-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="397c2-167">informationUrl</span></span>|<span data-ttu-id="397c2-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-168">String</span></span>|<span data-ttu-id="397c2-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="397c2-169">The more information Url.</span></span> <span data-ttu-id="397c2-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-171">owner</span><span class="sxs-lookup"><span data-stu-id="397c2-171">owner</span></span>|<span data-ttu-id="397c2-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-172">String</span></span>|<span data-ttu-id="397c2-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="397c2-173">The owner of the app.</span></span> <span data-ttu-id="397c2-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-175">developer</span><span class="sxs-lookup"><span data-stu-id="397c2-175">developer</span></span>|<span data-ttu-id="397c2-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-176">String</span></span>|<span data-ttu-id="397c2-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="397c2-177">The developer of the app.</span></span> <span data-ttu-id="397c2-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-179">notes</span><span class="sxs-lookup"><span data-stu-id="397c2-179">notes</span></span>|<span data-ttu-id="397c2-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-180">String</span></span>|<span data-ttu-id="397c2-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="397c2-181">Notes for the app.</span></span> <span data-ttu-id="397c2-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="397c2-183">uploadState</span></span>|<span data-ttu-id="397c2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="397c2-184">Int32</span></span>|<span data-ttu-id="397c2-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="397c2-185">The upload state.</span></span> <span data-ttu-id="397c2-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="397c2-187">publishingState</span></span>|[<span data-ttu-id="397c2-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="397c2-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="397c2-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="397c2-189">The publishing state for the app.</span></span> <span data-ttu-id="397c2-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="397c2-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="397c2-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="397c2-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="397c2-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="397c2-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="397c2-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="397c2-193">isAssigned</span></span>|<span data-ttu-id="397c2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="397c2-194">Boolean</span></span>|<span data-ttu-id="397c2-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="397c2-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="397c2-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="397c2-197">roleScopeTagIds</span></span>|<span data-ttu-id="397c2-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="397c2-198">String collection</span></span>|<span data-ttu-id="397c2-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="397c2-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="397c2-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="397c2-201">dependentAppCount</span></span>|<span data-ttu-id="397c2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="397c2-202">Int32</span></span>|<span data-ttu-id="397c2-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="397c2-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="397c2-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="397c2-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="397c2-205">committedContentVersion</span></span>|<span data-ttu-id="397c2-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-206">String</span></span>|<span data-ttu-id="397c2-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="397c2-207">The internal committed content version.</span></span> <span data-ttu-id="397c2-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="397c2-209">fileName</span><span class="sxs-lookup"><span data-stu-id="397c2-209">fileName</span></span>|<span data-ttu-id="397c2-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-210">String</span></span>|<span data-ttu-id="397c2-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="397c2-211">The name of the main Lob application file.</span></span> <span data-ttu-id="397c2-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="397c2-213">size</span><span class="sxs-lookup"><span data-stu-id="397c2-213">size</span></span>|<span data-ttu-id="397c2-214">Int64</span><span class="sxs-lookup"><span data-stu-id="397c2-214">Int64</span></span>|<span data-ttu-id="397c2-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="397c2-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="397c2-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="397c2-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="397c2-217">packageId</span><span class="sxs-lookup"><span data-stu-id="397c2-217">packageId</span></span>|<span data-ttu-id="397c2-218">String</span><span class="sxs-lookup"><span data-stu-id="397c2-218">String</span></span>|<span data-ttu-id="397c2-219">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="397c2-219">The package identifier.</span></span>|
|<span data-ttu-id="397c2-220">identityName</span><span class="sxs-lookup"><span data-stu-id="397c2-220">identityName</span></span>|<span data-ttu-id="397c2-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-221">String</span></span>|<span data-ttu-id="397c2-222">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="397c2-222">The Identity Name.</span></span>|
|<span data-ttu-id="397c2-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="397c2-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="397c2-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="397c2-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="397c2-225">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="397c2-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="397c2-226">versionName</span><span class="sxs-lookup"><span data-stu-id="397c2-226">versionName</span></span>|<span data-ttu-id="397c2-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-227">String</span></span>|<span data-ttu-id="397c2-228">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="397c2-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="397c2-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="397c2-229">versionCode</span></span>|<span data-ttu-id="397c2-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397c2-230">String</span></span>|<span data-ttu-id="397c2-231">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="397c2-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="397c2-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="397c2-232">identityVersion</span></span>|<span data-ttu-id="397c2-233">String</span><span class="sxs-lookup"><span data-stu-id="397c2-233">String</span></span>|<span data-ttu-id="397c2-234">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="397c2-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="397c2-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="397c2-235">Response</span></span>
<span data-ttu-id="397c2-236">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="397c2-236">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="397c2-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="397c2-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="397c2-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="397c2-238">Request</span></span>
<span data-ttu-id="397c2-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="397c2-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="397c2-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="397c2-240">Response</span></span>
<span data-ttu-id="397c2-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="397c2-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





