---
title: Criar win32LobApp
description: Criar um novo objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f805e9c41aacbc6c12cc44ad84f2e05db5b4d14
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793266"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="b966d-103">Criar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="b966d-103">Create win32LobApp</span></span>

<span data-ttu-id="b966d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b966d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b966d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b966d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b966d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b966d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b966d-107">Criar um novo objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b966d-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b966d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b966d-108">Prerequisites</span></span>
<span data-ttu-id="b966d-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b966d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b966d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b966d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b966d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b966d-111">Permission type</span></span>|<span data-ttu-id="b966d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b966d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b966d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b966d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b966d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b966d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b966d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b966d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b966d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b966d-116">Not supported.</span></span>|
|<span data-ttu-id="b966d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b966d-117">Application</span></span>|<span data-ttu-id="b966d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b966d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b966d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b966d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b966d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b966d-120">Request headers</span></span>
|<span data-ttu-id="b966d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b966d-121">Header</span></span>|<span data-ttu-id="b966d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b966d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b966d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b966d-123">Authorization</span></span>|<span data-ttu-id="b966d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b966d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b966d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b966d-125">Accept</span></span>|<span data-ttu-id="b966d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b966d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b966d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b966d-127">Request body</span></span>
<span data-ttu-id="b966d-128">No corpo da solicitação, forneça uma representação JSON do objeto win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="b966d-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="b966d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="b966d-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="b966d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b966d-130">Property</span></span>|<span data-ttu-id="b966d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b966d-131">Type</span></span>|<span data-ttu-id="b966d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b966d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b966d-133">id</span><span class="sxs-lookup"><span data-stu-id="b966d-133">id</span></span>|<span data-ttu-id="b966d-134">String</span><span class="sxs-lookup"><span data-stu-id="b966d-134">String</span></span>|<span data-ttu-id="b966d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b966d-135">Key of the entity.</span></span> <span data-ttu-id="b966d-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b966d-137">displayName</span></span>|<span data-ttu-id="b966d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b966d-138">String</span></span>|<span data-ttu-id="b966d-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b966d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b966d-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-141">description</span><span class="sxs-lookup"><span data-stu-id="b966d-141">description</span></span>|<span data-ttu-id="b966d-142">String</span><span class="sxs-lookup"><span data-stu-id="b966d-142">String</span></span>|<span data-ttu-id="b966d-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-143">The description of the app.</span></span> <span data-ttu-id="b966d-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-145">publicador</span><span class="sxs-lookup"><span data-stu-id="b966d-145">publisher</span></span>|<span data-ttu-id="b966d-146">String</span><span class="sxs-lookup"><span data-stu-id="b966d-146">String</span></span>|<span data-ttu-id="b966d-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-147">The publisher of the app.</span></span> <span data-ttu-id="b966d-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b966d-149">largeIcon</span></span>|[<span data-ttu-id="b966d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b966d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b966d-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b966d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b966d-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b966d-153">createdDateTime</span></span>|<span data-ttu-id="b966d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b966d-154">DateTimeOffset</span></span>|<span data-ttu-id="b966d-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-155">The date and time the app was created.</span></span> <span data-ttu-id="b966d-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b966d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b966d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b966d-158">DateTimeOffset</span></span>|<span data-ttu-id="b966d-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b966d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b966d-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b966d-161">isFeatured</span></span>|<span data-ttu-id="b966d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b966d-162">Boolean</span></span>|<span data-ttu-id="b966d-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b966d-164">privacyInformationUrl</span></span>|<span data-ttu-id="b966d-165">String</span><span class="sxs-lookup"><span data-stu-id="b966d-165">String</span></span>|<span data-ttu-id="b966d-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b966d-166">The privacy statement Url.</span></span> <span data-ttu-id="b966d-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b966d-168">informationUrl</span></span>|<span data-ttu-id="b966d-169">String</span><span class="sxs-lookup"><span data-stu-id="b966d-169">String</span></span>|<span data-ttu-id="b966d-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b966d-170">The more information Url.</span></span> <span data-ttu-id="b966d-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-172">owner</span><span class="sxs-lookup"><span data-stu-id="b966d-172">owner</span></span>|<span data-ttu-id="b966d-173">String</span><span class="sxs-lookup"><span data-stu-id="b966d-173">String</span></span>|<span data-ttu-id="b966d-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b966d-174">The owner of the app.</span></span> <span data-ttu-id="b966d-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-176">developer</span><span class="sxs-lookup"><span data-stu-id="b966d-176">developer</span></span>|<span data-ttu-id="b966d-177">String</span><span class="sxs-lookup"><span data-stu-id="b966d-177">String</span></span>|<span data-ttu-id="b966d-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-178">The developer of the app.</span></span> <span data-ttu-id="b966d-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-180">notes</span><span class="sxs-lookup"><span data-stu-id="b966d-180">notes</span></span>|<span data-ttu-id="b966d-181">String</span><span class="sxs-lookup"><span data-stu-id="b966d-181">String</span></span>|<span data-ttu-id="b966d-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-182">Notes for the app.</span></span> <span data-ttu-id="b966d-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b966d-184">uploadState</span></span>|<span data-ttu-id="b966d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b966d-185">Int32</span></span>|<span data-ttu-id="b966d-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="b966d-186">The upload state.</span></span> <span data-ttu-id="b966d-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b966d-188">publishingState</span></span>|[<span data-ttu-id="b966d-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b966d-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b966d-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-190">The publishing state for the app.</span></span> <span data-ttu-id="b966d-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b966d-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b966d-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b966d-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b966d-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b966d-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b966d-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b966d-194">isAssigned</span></span>|<span data-ttu-id="b966d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b966d-195">Boolean</span></span>|<span data-ttu-id="b966d-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="b966d-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b966d-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b966d-198">roleScopeTagIds</span></span>|<span data-ttu-id="b966d-199">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b966d-199">String collection</span></span>|<span data-ttu-id="b966d-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b966d-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b966d-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b966d-202">dependentAppCount</span></span>|<span data-ttu-id="b966d-203">Int32</span><span class="sxs-lookup"><span data-stu-id="b966d-203">Int32</span></span>|<span data-ttu-id="b966d-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="b966d-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b966d-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b966d-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b966d-206">committedContentVersion</span></span>|<span data-ttu-id="b966d-207">String</span><span class="sxs-lookup"><span data-stu-id="b966d-207">String</span></span>|<span data-ttu-id="b966d-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="b966d-208">The internal committed content version.</span></span> <span data-ttu-id="b966d-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b966d-210">fileName</span><span class="sxs-lookup"><span data-stu-id="b966d-210">fileName</span></span>|<span data-ttu-id="b966d-211">String</span><span class="sxs-lookup"><span data-stu-id="b966d-211">String</span></span>|<span data-ttu-id="b966d-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="b966d-212">The name of the main Lob application file.</span></span> <span data-ttu-id="b966d-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b966d-214">size</span><span class="sxs-lookup"><span data-stu-id="b966d-214">size</span></span>|<span data-ttu-id="b966d-215">Int64</span><span class="sxs-lookup"><span data-stu-id="b966d-215">Int64</span></span>|<span data-ttu-id="b966d-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="b966d-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="b966d-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b966d-218">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="b966d-218">installCommandLine</span></span>|<span data-ttu-id="b966d-219">String</span><span class="sxs-lookup"><span data-stu-id="b966d-219">String</span></span>|<span data-ttu-id="b966d-220">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="b966d-220">The command line to install this app</span></span>|
|<span data-ttu-id="b966d-221">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="b966d-221">uninstallCommandLine</span></span>|<span data-ttu-id="b966d-222">String</span><span class="sxs-lookup"><span data-stu-id="b966d-222">String</span></span>|<span data-ttu-id="b966d-223">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="b966d-223">The command line to uninstall this app</span></span>|
|<span data-ttu-id="b966d-224">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b966d-224">applicableArchitectures</span></span>|[<span data-ttu-id="b966d-225">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b966d-225">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b966d-226">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b966d-226">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b966d-227">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="b966d-227">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b966d-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b966d-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b966d-229">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b966d-229">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b966d-230">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b966d-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b966d-231">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="b966d-231">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="b966d-232">Int32</span><span class="sxs-lookup"><span data-stu-id="b966d-232">Int32</span></span>|<span data-ttu-id="b966d-233">O valor para o espaço livre mínimo em disco necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-233">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="b966d-234">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="b966d-234">minimumMemoryInMB</span></span>|<span data-ttu-id="b966d-235">Int32</span><span class="sxs-lookup"><span data-stu-id="b966d-235">Int32</span></span>|<span data-ttu-id="b966d-236">O valor da memória física mínima exigida para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-236">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="b966d-237">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="b966d-237">minimumNumberOfProcessors</span></span>|<span data-ttu-id="b966d-238">Int32</span><span class="sxs-lookup"><span data-stu-id="b966d-238">Int32</span></span>|<span data-ttu-id="b966d-239">O valor para o número mínimo de processadores necessários para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-239">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="b966d-240">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="b966d-240">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="b966d-241">Int32</span><span class="sxs-lookup"><span data-stu-id="b966d-241">Int32</span></span>|<span data-ttu-id="b966d-242">O valor para a velocidade de CPU mínima necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-242">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="b966d-243">detectionRules</span><span class="sxs-lookup"><span data-stu-id="b966d-243">detectionRules</span></span>|<span data-ttu-id="b966d-244">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="b966d-245">As regras de detecção para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="b966d-245">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b966d-246">requirementRules</span><span class="sxs-lookup"><span data-stu-id="b966d-246">requirementRules</span></span>|<span data-ttu-id="b966d-247">coleção [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="b966d-248">As regras de requisito para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="b966d-248">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b966d-249">regras</span><span class="sxs-lookup"><span data-stu-id="b966d-249">rules</span></span>|<span data-ttu-id="b966d-250">coleção [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-250">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="b966d-251">As regras de detecção e requisitos para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-251">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="b966d-252">installExperience</span><span class="sxs-lookup"><span data-stu-id="b966d-252">installExperience</span></span>|[<span data-ttu-id="b966d-253">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="b966d-253">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="b966d-254">A experiência de instalação para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b966d-254">The install experience for this app.</span></span>|
|<span data-ttu-id="b966d-255">returnCodes</span><span class="sxs-lookup"><span data-stu-id="b966d-255">returnCodes</span></span>|<span data-ttu-id="b966d-256">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="b966d-256">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="b966d-257">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="b966d-257">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="b966d-258">msiInformation</span><span class="sxs-lookup"><span data-stu-id="b966d-258">msiInformation</span></span>|[<span data-ttu-id="b966d-259">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="b966d-259">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="b966d-260">Os detalhes do MSI, se este aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="b966d-260">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="b966d-261">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="b966d-261">setupFilePath</span></span>|<span data-ttu-id="b966d-262">String</span><span class="sxs-lookup"><span data-stu-id="b966d-262">String</span></span>|<span data-ttu-id="b966d-263">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="b966d-263">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="b966d-264">installLanguage</span><span class="sxs-lookup"><span data-stu-id="b966d-264">installLanguage</span></span>|<span data-ttu-id="b966d-265">String</span><span class="sxs-lookup"><span data-stu-id="b966d-265">String</span></span>|<span data-ttu-id="b966d-266">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b966d-266">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b966d-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="b966d-267">Response</span></span>
<span data-ttu-id="b966d-268">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b966d-268">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b966d-269">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b966d-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="b966d-270">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b966d-270">Request</span></span>
<span data-ttu-id="b966d-271">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b966d-271">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 3224

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```

### <a name="response"></a><span data-ttu-id="b966d-272">Resposta</span><span class="sxs-lookup"><span data-stu-id="b966d-272">Response</span></span>
<span data-ttu-id="b966d-273">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b966d-273">Here is an example of the response.</span></span> <span data-ttu-id="b966d-274">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b966d-274">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b966d-275">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b966d-275">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3396

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```



