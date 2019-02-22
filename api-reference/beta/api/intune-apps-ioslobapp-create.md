---
title: Criar iosLobApp
description: Cria um novo objeto iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e72dcb4623c3505e297512f370b4a19b14ff3846
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169437"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="0077c-103">Criar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="0077c-103">Create iosLobApp</span></span>

> <span data-ttu-id="0077c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0077c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0077c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0077c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0077c-106">Cria um novo objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0077c-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0077c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0077c-107">Prerequisites</span></span>
<span data-ttu-id="0077c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0077c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0077c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0077c-110">Permission type</span></span>|<span data-ttu-id="0077c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0077c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0077c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0077c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0077c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0077c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0077c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0077c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0077c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0077c-115">Not supported.</span></span>|
|<span data-ttu-id="0077c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0077c-116">Application</span></span>|<span data-ttu-id="0077c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0077c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0077c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0077c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0077c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0077c-119">Request headers</span></span>
|<span data-ttu-id="0077c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0077c-120">Header</span></span>|<span data-ttu-id="0077c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0077c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0077c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0077c-122">Authorization</span></span>|<span data-ttu-id="0077c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0077c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0077c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0077c-124">Accept</span></span>|<span data-ttu-id="0077c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0077c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0077c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0077c-126">Request body</span></span>
<span data-ttu-id="0077c-127">No corpo da solicitação, forneça uma representação JSON do objeto iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="0077c-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="0077c-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="0077c-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="0077c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0077c-129">Property</span></span>|<span data-ttu-id="0077c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0077c-130">Type</span></span>|<span data-ttu-id="0077c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0077c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0077c-132">id</span><span class="sxs-lookup"><span data-stu-id="0077c-132">id</span></span>|<span data-ttu-id="0077c-133">String</span><span class="sxs-lookup"><span data-stu-id="0077c-133">String</span></span>|<span data-ttu-id="0077c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0077c-134">Key of the entity.</span></span> <span data-ttu-id="0077c-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0077c-136">displayName</span></span>|<span data-ttu-id="0077c-137">String</span><span class="sxs-lookup"><span data-stu-id="0077c-137">String</span></span>|<span data-ttu-id="0077c-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0077c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0077c-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-140">description</span><span class="sxs-lookup"><span data-stu-id="0077c-140">description</span></span>|<span data-ttu-id="0077c-141">String</span><span class="sxs-lookup"><span data-stu-id="0077c-141">String</span></span>|<span data-ttu-id="0077c-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0077c-142">The description of the app.</span></span> <span data-ttu-id="0077c-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0077c-144">publisher</span></span>|<span data-ttu-id="0077c-145">String</span><span class="sxs-lookup"><span data-stu-id="0077c-145">String</span></span>|<span data-ttu-id="0077c-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0077c-146">The publisher of the app.</span></span> <span data-ttu-id="0077c-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0077c-148">largeIcon</span></span>|[<span data-ttu-id="0077c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0077c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0077c-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0077c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0077c-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0077c-152">createdDateTime</span></span>|<span data-ttu-id="0077c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0077c-153">DateTimeOffset</span></span>|<span data-ttu-id="0077c-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0077c-154">The date and time the app was created.</span></span> <span data-ttu-id="0077c-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0077c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0077c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0077c-157">DateTimeOffset</span></span>|<span data-ttu-id="0077c-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0077c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0077c-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0077c-160">isFeatured</span></span>|<span data-ttu-id="0077c-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="0077c-161">Boolean</span></span>|<span data-ttu-id="0077c-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0077c-163">privacyInformationUrl</span></span>|<span data-ttu-id="0077c-164">String</span><span class="sxs-lookup"><span data-stu-id="0077c-164">String</span></span>|<span data-ttu-id="0077c-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0077c-165">The privacy statement Url.</span></span> <span data-ttu-id="0077c-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0077c-167">informationUrl</span></span>|<span data-ttu-id="0077c-168">String</span><span class="sxs-lookup"><span data-stu-id="0077c-168">String</span></span>|<span data-ttu-id="0077c-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0077c-169">The more information Url.</span></span> <span data-ttu-id="0077c-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-171">owner</span><span class="sxs-lookup"><span data-stu-id="0077c-171">owner</span></span>|<span data-ttu-id="0077c-172">String</span><span class="sxs-lookup"><span data-stu-id="0077c-172">String</span></span>|<span data-ttu-id="0077c-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0077c-173">The owner of the app.</span></span> <span data-ttu-id="0077c-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-175">developer</span><span class="sxs-lookup"><span data-stu-id="0077c-175">developer</span></span>|<span data-ttu-id="0077c-176">String</span><span class="sxs-lookup"><span data-stu-id="0077c-176">String</span></span>|<span data-ttu-id="0077c-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0077c-177">The developer of the app.</span></span> <span data-ttu-id="0077c-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-179">Observações</span><span class="sxs-lookup"><span data-stu-id="0077c-179">notes</span></span>|<span data-ttu-id="0077c-180">String</span><span class="sxs-lookup"><span data-stu-id="0077c-180">String</span></span>|<span data-ttu-id="0077c-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0077c-181">Notes for the app.</span></span> <span data-ttu-id="0077c-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0077c-183">uploadState</span></span>|<span data-ttu-id="0077c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0077c-184">Int32</span></span>|<span data-ttu-id="0077c-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="0077c-185">The upload state.</span></span> <span data-ttu-id="0077c-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0077c-187">publishingState</span></span>|[<span data-ttu-id="0077c-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0077c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0077c-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0077c-189">The publishing state for the app.</span></span> <span data-ttu-id="0077c-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0077c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0077c-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0077c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0077c-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0077c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0077c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0077c-193">isAssigned</span></span>|<span data-ttu-id="0077c-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="0077c-194">Boolean</span></span>|<span data-ttu-id="0077c-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="0077c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0077c-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0077c-197">roleScopeTagIds</span></span>|<span data-ttu-id="0077c-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0077c-198">String collection</span></span>|<span data-ttu-id="0077c-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0077c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0077c-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0077c-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0077c-201">committedContentVersion</span></span>|<span data-ttu-id="0077c-202">String</span><span class="sxs-lookup"><span data-stu-id="0077c-202">String</span></span>|<span data-ttu-id="0077c-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="0077c-203">The internal committed content version.</span></span> <span data-ttu-id="0077c-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0077c-205">fileName</span><span class="sxs-lookup"><span data-stu-id="0077c-205">fileName</span></span>|<span data-ttu-id="0077c-206">String</span><span class="sxs-lookup"><span data-stu-id="0077c-206">String</span></span>|<span data-ttu-id="0077c-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="0077c-207">The name of the main Lob application file.</span></span> <span data-ttu-id="0077c-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0077c-209">size</span><span class="sxs-lookup"><span data-stu-id="0077c-209">size</span></span>|<span data-ttu-id="0077c-210">Int64</span><span class="sxs-lookup"><span data-stu-id="0077c-210">Int64</span></span>|<span data-ttu-id="0077c-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="0077c-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="0077c-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0077c-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0077c-213">bundleId</span><span class="sxs-lookup"><span data-stu-id="0077c-213">bundleId</span></span>|<span data-ttu-id="0077c-214">String</span><span class="sxs-lookup"><span data-stu-id="0077c-214">String</span></span>|<span data-ttu-id="0077c-215">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0077c-215">The Identity Name.</span></span>|
|<span data-ttu-id="0077c-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="0077c-216">applicableDeviceType</span></span>|[<span data-ttu-id="0077c-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="0077c-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="0077c-218">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="0077c-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="0077c-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0077c-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0077c-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0077c-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="0077c-221">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="0077c-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0077c-222">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0077c-222">expirationDateTime</span></span>|<span data-ttu-id="0077c-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0077c-223">DateTimeOffset</span></span>|<span data-ttu-id="0077c-224">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="0077c-224">The expiration time.</span></span>|
|<span data-ttu-id="0077c-225">versionNumber</span><span class="sxs-lookup"><span data-stu-id="0077c-225">versionNumber</span></span>|<span data-ttu-id="0077c-226">String</span><span class="sxs-lookup"><span data-stu-id="0077c-226">String</span></span>|<span data-ttu-id="0077c-227">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="0077c-227">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0077c-228">buildNumber</span><span class="sxs-lookup"><span data-stu-id="0077c-228">buildNumber</span></span>|<span data-ttu-id="0077c-229">String</span><span class="sxs-lookup"><span data-stu-id="0077c-229">String</span></span>|<span data-ttu-id="0077c-230">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="0077c-230">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0077c-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="0077c-231">identityVersion</span></span>|<span data-ttu-id="0077c-232">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0077c-232">String</span></span>|<span data-ttu-id="0077c-233">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="0077c-233">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="0077c-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="0077c-234">Response</span></span>
<span data-ttu-id="0077c-235">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0077c-235">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0077c-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0077c-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="0077c-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0077c-237">Request</span></span>
<span data-ttu-id="0077c-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0077c-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="0077c-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="0077c-239">Response</span></span>
<span data-ttu-id="0077c-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0077c-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




