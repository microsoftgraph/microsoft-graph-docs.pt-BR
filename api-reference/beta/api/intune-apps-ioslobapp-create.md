---
title: Criar iosLobApp
description: Cria um novo objeto iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b33d36a16c375bc80524f4696bb3fc459834fe46
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791947"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="910aa-103">Criar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="910aa-103">Create iosLobApp</span></span>

> <span data-ttu-id="910aa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="910aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="910aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="910aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="910aa-106">Cria um novo objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="910aa-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="910aa-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="910aa-107">Prerequisites</span></span>
<span data-ttu-id="910aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="910aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="910aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="910aa-110">Permission type</span></span>|<span data-ttu-id="910aa-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="910aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="910aa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="910aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="910aa-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="910aa-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="910aa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="910aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="910aa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="910aa-115">Not supported.</span></span>|
|<span data-ttu-id="910aa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="910aa-116">Application</span></span>|<span data-ttu-id="910aa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="910aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="910aa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="910aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="910aa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="910aa-119">Request headers</span></span>
|<span data-ttu-id="910aa-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="910aa-120">Header</span></span>|<span data-ttu-id="910aa-121">Valor</span><span class="sxs-lookup"><span data-stu-id="910aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="910aa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="910aa-122">Authorization</span></span>|<span data-ttu-id="910aa-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="910aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="910aa-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="910aa-124">Accept</span></span>|<span data-ttu-id="910aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="910aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="910aa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="910aa-126">Request body</span></span>
<span data-ttu-id="910aa-127">No corpo da solicitação, forneça uma representação JSON do objeto iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="910aa-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="910aa-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="910aa-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="910aa-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="910aa-129">Property</span></span>|<span data-ttu-id="910aa-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="910aa-130">Type</span></span>|<span data-ttu-id="910aa-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="910aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="910aa-132">id</span><span class="sxs-lookup"><span data-stu-id="910aa-132">id</span></span>|<span data-ttu-id="910aa-133">String</span><span class="sxs-lookup"><span data-stu-id="910aa-133">String</span></span>|<span data-ttu-id="910aa-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="910aa-134">Key of the entity.</span></span> <span data-ttu-id="910aa-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="910aa-136">displayName</span></span>|<span data-ttu-id="910aa-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-137">String</span></span>|<span data-ttu-id="910aa-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="910aa-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="910aa-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-140">description</span><span class="sxs-lookup"><span data-stu-id="910aa-140">description</span></span>|<span data-ttu-id="910aa-141">String</span><span class="sxs-lookup"><span data-stu-id="910aa-141">String</span></span>|<span data-ttu-id="910aa-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="910aa-142">The description of the app.</span></span> <span data-ttu-id="910aa-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-144">publicador</span><span class="sxs-lookup"><span data-stu-id="910aa-144">publisher</span></span>|<span data-ttu-id="910aa-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-145">String</span></span>|<span data-ttu-id="910aa-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="910aa-146">The publisher of the app.</span></span> <span data-ttu-id="910aa-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="910aa-148">largeIcon</span></span>|[<span data-ttu-id="910aa-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="910aa-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="910aa-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="910aa-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="910aa-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="910aa-152">createdDateTime</span></span>|<span data-ttu-id="910aa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910aa-153">DateTimeOffset</span></span>|<span data-ttu-id="910aa-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="910aa-154">The date and time the app was created.</span></span> <span data-ttu-id="910aa-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="910aa-156">lastModifiedDateTime</span></span>|<span data-ttu-id="910aa-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910aa-157">DateTimeOffset</span></span>|<span data-ttu-id="910aa-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="910aa-158">The date and time the app was last modified.</span></span> <span data-ttu-id="910aa-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="910aa-160">isFeatured</span></span>|<span data-ttu-id="910aa-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="910aa-161">Boolean</span></span>|<span data-ttu-id="910aa-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="910aa-163">privacyInformationUrl</span></span>|<span data-ttu-id="910aa-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-164">String</span></span>|<span data-ttu-id="910aa-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="910aa-165">The privacy statement Url.</span></span> <span data-ttu-id="910aa-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="910aa-167">informationUrl</span></span>|<span data-ttu-id="910aa-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-168">String</span></span>|<span data-ttu-id="910aa-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="910aa-169">The more information Url.</span></span> <span data-ttu-id="910aa-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-171">owner</span><span class="sxs-lookup"><span data-stu-id="910aa-171">owner</span></span>|<span data-ttu-id="910aa-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-172">String</span></span>|<span data-ttu-id="910aa-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="910aa-173">The owner of the app.</span></span> <span data-ttu-id="910aa-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-175">developer</span><span class="sxs-lookup"><span data-stu-id="910aa-175">developer</span></span>|<span data-ttu-id="910aa-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-176">String</span></span>|<span data-ttu-id="910aa-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="910aa-177">The developer of the app.</span></span> <span data-ttu-id="910aa-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-179">notes</span><span class="sxs-lookup"><span data-stu-id="910aa-179">notes</span></span>|<span data-ttu-id="910aa-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-180">String</span></span>|<span data-ttu-id="910aa-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="910aa-181">Notes for the app.</span></span> <span data-ttu-id="910aa-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="910aa-183">uploadState</span></span>|<span data-ttu-id="910aa-184">Int32</span><span class="sxs-lookup"><span data-stu-id="910aa-184">Int32</span></span>|<span data-ttu-id="910aa-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="910aa-185">The upload state.</span></span> <span data-ttu-id="910aa-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="910aa-187">publishingState</span></span>|[<span data-ttu-id="910aa-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="910aa-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="910aa-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="910aa-189">The publishing state for the app.</span></span> <span data-ttu-id="910aa-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="910aa-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="910aa-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="910aa-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="910aa-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="910aa-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="910aa-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="910aa-193">isAssigned</span></span>|<span data-ttu-id="910aa-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="910aa-194">Boolean</span></span>|<span data-ttu-id="910aa-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="910aa-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="910aa-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="910aa-197">roleScopeTagIds</span></span>|<span data-ttu-id="910aa-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="910aa-198">String collection</span></span>|<span data-ttu-id="910aa-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="910aa-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="910aa-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="910aa-201">dependentAppCount</span></span>|<span data-ttu-id="910aa-202">Int32</span><span class="sxs-lookup"><span data-stu-id="910aa-202">Int32</span></span>|<span data-ttu-id="910aa-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="910aa-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="910aa-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="910aa-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="910aa-205">committedContentVersion</span></span>|<span data-ttu-id="910aa-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-206">String</span></span>|<span data-ttu-id="910aa-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="910aa-207">The internal committed content version.</span></span> <span data-ttu-id="910aa-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="910aa-209">fileName</span><span class="sxs-lookup"><span data-stu-id="910aa-209">fileName</span></span>|<span data-ttu-id="910aa-210">String</span><span class="sxs-lookup"><span data-stu-id="910aa-210">String</span></span>|<span data-ttu-id="910aa-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="910aa-211">The name of the main Lob application file.</span></span> <span data-ttu-id="910aa-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="910aa-213">size</span><span class="sxs-lookup"><span data-stu-id="910aa-213">size</span></span>|<span data-ttu-id="910aa-214">Int64</span><span class="sxs-lookup"><span data-stu-id="910aa-214">Int64</span></span>|<span data-ttu-id="910aa-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="910aa-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="910aa-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="910aa-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="910aa-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="910aa-217">bundleId</span></span>|<span data-ttu-id="910aa-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-218">String</span></span>|<span data-ttu-id="910aa-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="910aa-219">The Identity Name.</span></span>|
|<span data-ttu-id="910aa-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="910aa-220">applicableDeviceType</span></span>|[<span data-ttu-id="910aa-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="910aa-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="910aa-222">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="910aa-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="910aa-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="910aa-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="910aa-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="910aa-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="910aa-225">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="910aa-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="910aa-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="910aa-226">expirationDateTime</span></span>|<span data-ttu-id="910aa-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910aa-227">DateTimeOffset</span></span>|<span data-ttu-id="910aa-228">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="910aa-228">The expiration time.</span></span>|
|<span data-ttu-id="910aa-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="910aa-229">versionNumber</span></span>|<span data-ttu-id="910aa-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-230">String</span></span>|<span data-ttu-id="910aa-231">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="910aa-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="910aa-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="910aa-232">buildNumber</span></span>|<span data-ttu-id="910aa-233">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="910aa-233">String</span></span>|<span data-ttu-id="910aa-234">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="910aa-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="910aa-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="910aa-235">identityVersion</span></span>|<span data-ttu-id="910aa-236">String</span><span class="sxs-lookup"><span data-stu-id="910aa-236">String</span></span>|<span data-ttu-id="910aa-237">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="910aa-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="910aa-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="910aa-238">Response</span></span>
<span data-ttu-id="910aa-239">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="910aa-239">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="910aa-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="910aa-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="910aa-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="910aa-241">Request</span></span>
<span data-ttu-id="910aa-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="910aa-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="910aa-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="910aa-243">Response</span></span>
<span data-ttu-id="910aa-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="910aa-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





