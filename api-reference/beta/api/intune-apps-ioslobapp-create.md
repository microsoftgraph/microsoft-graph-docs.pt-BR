---
title: Criar iosLobApp
description: Cria um novo objeto iosLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad0df70f908c42084d8f9769c1b01bf8d65929aa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535433"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="386ba-103">Criar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="386ba-103">Create iosLobApp</span></span>

> <span data-ttu-id="386ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="386ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="386ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="386ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="386ba-106">Cria um novo objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="386ba-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="386ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="386ba-107">Prerequisites</span></span>
<span data-ttu-id="386ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="386ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="386ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="386ba-110">Permission type</span></span>|<span data-ttu-id="386ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="386ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="386ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="386ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="386ba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386ba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="386ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="386ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="386ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="386ba-115">Not supported.</span></span>|
|<span data-ttu-id="386ba-116">Application</span><span class="sxs-lookup"><span data-stu-id="386ba-116">Application</span></span>|<span data-ttu-id="386ba-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386ba-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="386ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="386ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="386ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="386ba-119">Request headers</span></span>
|<span data-ttu-id="386ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="386ba-120">Header</span></span>|<span data-ttu-id="386ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="386ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="386ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="386ba-122">Authorization</span></span>|<span data-ttu-id="386ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="386ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="386ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="386ba-124">Accept</span></span>|<span data-ttu-id="386ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="386ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="386ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="386ba-126">Request body</span></span>
<span data-ttu-id="386ba-127">No corpo da solicitação, forneça uma representação JSON do objeto iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="386ba-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="386ba-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="386ba-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="386ba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="386ba-129">Property</span></span>|<span data-ttu-id="386ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="386ba-130">Type</span></span>|<span data-ttu-id="386ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="386ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="386ba-132">id</span><span class="sxs-lookup"><span data-stu-id="386ba-132">id</span></span>|<span data-ttu-id="386ba-133">String</span><span class="sxs-lookup"><span data-stu-id="386ba-133">String</span></span>|<span data-ttu-id="386ba-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="386ba-134">Key of the entity.</span></span> <span data-ttu-id="386ba-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="386ba-136">displayName</span></span>|<span data-ttu-id="386ba-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-137">String</span></span>|<span data-ttu-id="386ba-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="386ba-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="386ba-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-140">description</span><span class="sxs-lookup"><span data-stu-id="386ba-140">description</span></span>|<span data-ttu-id="386ba-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-141">String</span></span>|<span data-ttu-id="386ba-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="386ba-142">The description of the app.</span></span> <span data-ttu-id="386ba-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-144">publicador</span><span class="sxs-lookup"><span data-stu-id="386ba-144">publisher</span></span>|<span data-ttu-id="386ba-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-145">String</span></span>|<span data-ttu-id="386ba-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="386ba-146">The publisher of the app.</span></span> <span data-ttu-id="386ba-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="386ba-148">largeIcon</span></span>|[<span data-ttu-id="386ba-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="386ba-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="386ba-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="386ba-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="386ba-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="386ba-152">createdDateTime</span></span>|<span data-ttu-id="386ba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="386ba-153">DateTimeOffset</span></span>|<span data-ttu-id="386ba-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="386ba-154">The date and time the app was created.</span></span> <span data-ttu-id="386ba-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="386ba-156">lastModifiedDateTime</span></span>|<span data-ttu-id="386ba-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="386ba-157">DateTimeOffset</span></span>|<span data-ttu-id="386ba-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="386ba-158">The date and time the app was last modified.</span></span> <span data-ttu-id="386ba-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="386ba-160">isFeatured</span></span>|<span data-ttu-id="386ba-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="386ba-161">Boolean</span></span>|<span data-ttu-id="386ba-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="386ba-163">privacyInformationUrl</span></span>|<span data-ttu-id="386ba-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-164">String</span></span>|<span data-ttu-id="386ba-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="386ba-165">The privacy statement Url.</span></span> <span data-ttu-id="386ba-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="386ba-167">informationUrl</span></span>|<span data-ttu-id="386ba-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-168">String</span></span>|<span data-ttu-id="386ba-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="386ba-169">The more information Url.</span></span> <span data-ttu-id="386ba-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-171">owner</span><span class="sxs-lookup"><span data-stu-id="386ba-171">owner</span></span>|<span data-ttu-id="386ba-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-172">String</span></span>|<span data-ttu-id="386ba-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="386ba-173">The owner of the app.</span></span> <span data-ttu-id="386ba-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-175">developer</span><span class="sxs-lookup"><span data-stu-id="386ba-175">developer</span></span>|<span data-ttu-id="386ba-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-176">String</span></span>|<span data-ttu-id="386ba-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="386ba-177">The developer of the app.</span></span> <span data-ttu-id="386ba-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-179">notes</span><span class="sxs-lookup"><span data-stu-id="386ba-179">notes</span></span>|<span data-ttu-id="386ba-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-180">String</span></span>|<span data-ttu-id="386ba-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="386ba-181">Notes for the app.</span></span> <span data-ttu-id="386ba-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="386ba-183">uploadState</span></span>|<span data-ttu-id="386ba-184">Int32</span><span class="sxs-lookup"><span data-stu-id="386ba-184">Int32</span></span>|<span data-ttu-id="386ba-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="386ba-185">The upload state.</span></span> <span data-ttu-id="386ba-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="386ba-187">publishingState</span></span>|[<span data-ttu-id="386ba-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="386ba-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="386ba-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="386ba-189">The publishing state for the app.</span></span> <span data-ttu-id="386ba-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="386ba-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="386ba-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="386ba-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="386ba-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="386ba-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="386ba-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="386ba-193">isAssigned</span></span>|<span data-ttu-id="386ba-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="386ba-194">Boolean</span></span>|<span data-ttu-id="386ba-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="386ba-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="386ba-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="386ba-197">roleScopeTagIds</span></span>|<span data-ttu-id="386ba-198">String collection</span><span class="sxs-lookup"><span data-stu-id="386ba-198">String collection</span></span>|<span data-ttu-id="386ba-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="386ba-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="386ba-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="386ba-201">dependentAppCount</span></span>|<span data-ttu-id="386ba-202">Int32</span><span class="sxs-lookup"><span data-stu-id="386ba-202">Int32</span></span>|<span data-ttu-id="386ba-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="386ba-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="386ba-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="386ba-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="386ba-205">committedContentVersion</span></span>|<span data-ttu-id="386ba-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-206">String</span></span>|<span data-ttu-id="386ba-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="386ba-207">The internal committed content version.</span></span> <span data-ttu-id="386ba-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="386ba-209">fileName</span><span class="sxs-lookup"><span data-stu-id="386ba-209">fileName</span></span>|<span data-ttu-id="386ba-210">String</span><span class="sxs-lookup"><span data-stu-id="386ba-210">String</span></span>|<span data-ttu-id="386ba-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="386ba-211">The name of the main Lob application file.</span></span> <span data-ttu-id="386ba-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="386ba-213">size</span><span class="sxs-lookup"><span data-stu-id="386ba-213">size</span></span>|<span data-ttu-id="386ba-214">Int64</span><span class="sxs-lookup"><span data-stu-id="386ba-214">Int64</span></span>|<span data-ttu-id="386ba-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="386ba-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="386ba-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="386ba-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="386ba-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="386ba-217">bundleId</span></span>|<span data-ttu-id="386ba-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-218">String</span></span>|<span data-ttu-id="386ba-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="386ba-219">The Identity Name.</span></span>|
|<span data-ttu-id="386ba-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="386ba-220">applicableDeviceType</span></span>|[<span data-ttu-id="386ba-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="386ba-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="386ba-222">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="386ba-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="386ba-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="386ba-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="386ba-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="386ba-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="386ba-225">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="386ba-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="386ba-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="386ba-226">expirationDateTime</span></span>|<span data-ttu-id="386ba-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="386ba-227">DateTimeOffset</span></span>|<span data-ttu-id="386ba-228">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="386ba-228">The expiration time.</span></span>|
|<span data-ttu-id="386ba-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="386ba-229">versionNumber</span></span>|<span data-ttu-id="386ba-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-230">String</span></span>|<span data-ttu-id="386ba-231">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="386ba-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="386ba-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="386ba-232">buildNumber</span></span>|<span data-ttu-id="386ba-233">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386ba-233">String</span></span>|<span data-ttu-id="386ba-234">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="386ba-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="386ba-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="386ba-235">identityVersion</span></span>|<span data-ttu-id="386ba-236">String</span><span class="sxs-lookup"><span data-stu-id="386ba-236">String</span></span>|<span data-ttu-id="386ba-237">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="386ba-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="386ba-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="386ba-238">Response</span></span>
<span data-ttu-id="386ba-239">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="386ba-239">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="386ba-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="386ba-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="386ba-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="386ba-241">Request</span></span>
<span data-ttu-id="386ba-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="386ba-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="386ba-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="386ba-243">Response</span></span>
<span data-ttu-id="386ba-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="386ba-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






