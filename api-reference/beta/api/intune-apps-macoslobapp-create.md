---
title: Criar macOSLobApp
description: Criar um novo objeto macOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 512693516b206802b147e8eb9dad0f918c329597
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330269"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="02302-103">Criar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="02302-103">Create macOSLobApp</span></span>

> <span data-ttu-id="02302-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02302-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02302-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02302-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02302-106">Criar um novo objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="02302-106">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02302-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02302-107">Prerequisites</span></span>
<span data-ttu-id="02302-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02302-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02302-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02302-110">Permission type</span></span>|<span data-ttu-id="02302-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02302-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02302-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02302-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02302-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02302-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02302-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02302-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02302-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02302-115">Not supported.</span></span>|
|<span data-ttu-id="02302-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02302-116">Application</span></span>|<span data-ttu-id="02302-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02302-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02302-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02302-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="02302-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02302-119">Request headers</span></span>
|<span data-ttu-id="02302-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02302-120">Header</span></span>|<span data-ttu-id="02302-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02302-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02302-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02302-122">Authorization</span></span>|<span data-ttu-id="02302-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02302-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02302-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02302-124">Accept</span></span>|<span data-ttu-id="02302-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02302-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02302-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02302-126">Request body</span></span>
<span data-ttu-id="02302-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="02302-127">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="02302-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="02302-128">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="02302-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02302-129">Property</span></span>|<span data-ttu-id="02302-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="02302-130">Type</span></span>|<span data-ttu-id="02302-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="02302-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02302-132">id</span><span class="sxs-lookup"><span data-stu-id="02302-132">id</span></span>|<span data-ttu-id="02302-133">String</span><span class="sxs-lookup"><span data-stu-id="02302-133">String</span></span>|<span data-ttu-id="02302-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02302-134">Key of the entity.</span></span> <span data-ttu-id="02302-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-136">displayName</span><span class="sxs-lookup"><span data-stu-id="02302-136">displayName</span></span>|<span data-ttu-id="02302-137">String</span><span class="sxs-lookup"><span data-stu-id="02302-137">String</span></span>|<span data-ttu-id="02302-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="02302-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="02302-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-140">descrição</span><span class="sxs-lookup"><span data-stu-id="02302-140">description</span></span>|<span data-ttu-id="02302-141">String</span><span class="sxs-lookup"><span data-stu-id="02302-141">String</span></span>|<span data-ttu-id="02302-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02302-142">The description of the app.</span></span> <span data-ttu-id="02302-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-144">publicador</span><span class="sxs-lookup"><span data-stu-id="02302-144">publisher</span></span>|<span data-ttu-id="02302-145">String</span><span class="sxs-lookup"><span data-stu-id="02302-145">String</span></span>|<span data-ttu-id="02302-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02302-146">The publisher of the app.</span></span> <span data-ttu-id="02302-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="02302-148">largeIcon</span></span>|[<span data-ttu-id="02302-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="02302-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="02302-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="02302-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="02302-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02302-152">createdDateTime</span></span>|<span data-ttu-id="02302-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02302-153">DateTimeOffset</span></span>|<span data-ttu-id="02302-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02302-154">The date and time the app was created.</span></span> <span data-ttu-id="02302-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02302-156">lastModifiedDateTime</span></span>|<span data-ttu-id="02302-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02302-157">DateTimeOffset</span></span>|<span data-ttu-id="02302-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="02302-158">The date and time the app was last modified.</span></span> <span data-ttu-id="02302-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="02302-160">isFeatured</span></span>|<span data-ttu-id="02302-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="02302-161">Boolean</span></span>|<span data-ttu-id="02302-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="02302-163">privacyInformationUrl</span></span>|<span data-ttu-id="02302-164">String</span><span class="sxs-lookup"><span data-stu-id="02302-164">String</span></span>|<span data-ttu-id="02302-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="02302-165">The privacy statement Url.</span></span> <span data-ttu-id="02302-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="02302-167">informationUrl</span></span>|<span data-ttu-id="02302-168">String</span><span class="sxs-lookup"><span data-stu-id="02302-168">String</span></span>|<span data-ttu-id="02302-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="02302-169">The more information Url.</span></span> <span data-ttu-id="02302-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-171">owner</span><span class="sxs-lookup"><span data-stu-id="02302-171">owner</span></span>|<span data-ttu-id="02302-172">String</span><span class="sxs-lookup"><span data-stu-id="02302-172">String</span></span>|<span data-ttu-id="02302-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="02302-173">The owner of the app.</span></span> <span data-ttu-id="02302-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-175">developer</span><span class="sxs-lookup"><span data-stu-id="02302-175">developer</span></span>|<span data-ttu-id="02302-176">String</span><span class="sxs-lookup"><span data-stu-id="02302-176">String</span></span>|<span data-ttu-id="02302-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02302-177">The developer of the app.</span></span> <span data-ttu-id="02302-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-179">notes</span><span class="sxs-lookup"><span data-stu-id="02302-179">notes</span></span>|<span data-ttu-id="02302-180">String</span><span class="sxs-lookup"><span data-stu-id="02302-180">String</span></span>|<span data-ttu-id="02302-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02302-181">Notes for the app.</span></span> <span data-ttu-id="02302-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="02302-183">uploadState</span></span>|<span data-ttu-id="02302-184">Int32</span><span class="sxs-lookup"><span data-stu-id="02302-184">Int32</span></span>|<span data-ttu-id="02302-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="02302-185">The upload state.</span></span> <span data-ttu-id="02302-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="02302-187">publishingState</span></span>|[<span data-ttu-id="02302-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="02302-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="02302-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02302-189">The publishing state for the app.</span></span> <span data-ttu-id="02302-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="02302-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="02302-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02302-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="02302-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="02302-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="02302-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="02302-193">isAssigned</span></span>|<span data-ttu-id="02302-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="02302-194">Boolean</span></span>|<span data-ttu-id="02302-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="02302-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="02302-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="02302-197">roleScopeTagIds</span></span>|<span data-ttu-id="02302-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="02302-198">String collection</span></span>|<span data-ttu-id="02302-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="02302-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="02302-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="02302-201">dependentAppCount</span></span>|<span data-ttu-id="02302-202">Int32</span><span class="sxs-lookup"><span data-stu-id="02302-202">Int32</span></span>|<span data-ttu-id="02302-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="02302-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="02302-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="02302-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="02302-205">committedContentVersion</span></span>|<span data-ttu-id="02302-206">String</span><span class="sxs-lookup"><span data-stu-id="02302-206">String</span></span>|<span data-ttu-id="02302-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="02302-207">The internal committed content version.</span></span> <span data-ttu-id="02302-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="02302-209">fileName</span><span class="sxs-lookup"><span data-stu-id="02302-209">fileName</span></span>|<span data-ttu-id="02302-210">String</span><span class="sxs-lookup"><span data-stu-id="02302-210">String</span></span>|<span data-ttu-id="02302-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="02302-211">The name of the main Lob application file.</span></span> <span data-ttu-id="02302-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="02302-213">size</span><span class="sxs-lookup"><span data-stu-id="02302-213">size</span></span>|<span data-ttu-id="02302-214">Int64</span><span class="sxs-lookup"><span data-stu-id="02302-214">Int64</span></span>|<span data-ttu-id="02302-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="02302-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="02302-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="02302-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="02302-217">bundleId</span></span>|<span data-ttu-id="02302-218">String</span><span class="sxs-lookup"><span data-stu-id="02302-218">String</span></span>|<span data-ttu-id="02302-219">A ID do pacote.</span><span class="sxs-lookup"><span data-stu-id="02302-219">The bundle id.</span></span>|
|<span data-ttu-id="02302-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="02302-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="02302-221">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="02302-221">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="02302-222">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="02302-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="02302-223">buildNumber</span><span class="sxs-lookup"><span data-stu-id="02302-223">buildNumber</span></span>|<span data-ttu-id="02302-224">String</span><span class="sxs-lookup"><span data-stu-id="02302-224">String</span></span>|<span data-ttu-id="02302-225">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="02302-225">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="02302-226">versionNumber</span><span class="sxs-lookup"><span data-stu-id="02302-226">versionNumber</span></span>|<span data-ttu-id="02302-227">String</span><span class="sxs-lookup"><span data-stu-id="02302-227">String</span></span>|<span data-ttu-id="02302-228">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="02302-228">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="02302-229">childApps</span><span class="sxs-lookup"><span data-stu-id="02302-229">childApps</span></span>|<span data-ttu-id="02302-230">coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="02302-230">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="02302-231">A lista de aplicativos neste pacote de pacotes</span><span class="sxs-lookup"><span data-stu-id="02302-231">The app list in this bundle package</span></span>|
|<span data-ttu-id="02302-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="02302-232">identityVersion</span></span>|<span data-ttu-id="02302-233">String</span><span class="sxs-lookup"><span data-stu-id="02302-233">String</span></span>|<span data-ttu-id="02302-234">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="02302-234">The identity version.</span></span>|
|<span data-ttu-id="02302-235">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="02302-235">md5HashChunkSize</span></span>|<span data-ttu-id="02302-236">Int32</span><span class="sxs-lookup"><span data-stu-id="02302-236">Int32</span></span>|<span data-ttu-id="02302-237">O tamanho da parte do hash MD5</span><span class="sxs-lookup"><span data-stu-id="02302-237">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="02302-238">md5Hash</span><span class="sxs-lookup"><span data-stu-id="02302-238">md5Hash</span></span>|<span data-ttu-id="02302-239">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="02302-239">String collection</span></span>|<span data-ttu-id="02302-240">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="02302-240">The MD5 hash codes</span></span>|
|<span data-ttu-id="02302-241">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="02302-241">ignoreVersionDetection</span></span>|<span data-ttu-id="02302-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="02302-242">Boolean</span></span>|<span data-ttu-id="02302-243">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02302-243">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="02302-244">Defina isso como true para aplicativos de linha de negócios (LoB) de macOS que usam um recurso de autoatualização.</span><span class="sxs-lookup"><span data-stu-id="02302-244">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="02302-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="02302-245">Response</span></span>
<span data-ttu-id="02302-246">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02302-246">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02302-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02302-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="02302-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02302-248">Request</span></span>
<span data-ttu-id="02302-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02302-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1574

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
    "v10_13": true
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

### <a name="response"></a><span data-ttu-id="02302-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="02302-250">Response</span></span>
<span data-ttu-id="02302-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02302-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1746

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
    "v10_13": true
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






