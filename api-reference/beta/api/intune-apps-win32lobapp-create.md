---
title: Criar win32LobApp
description: Criar um novo objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c367c8f14002efce5132210e0c695ad00f850de
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123460"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="06a80-103">Criar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="06a80-103">Create win32LobApp</span></span>

<span data-ttu-id="06a80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06a80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06a80-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06a80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06a80-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06a80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06a80-107">Criar um novo objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="06a80-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06a80-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06a80-108">Prerequisites</span></span>
<span data-ttu-id="06a80-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="06a80-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="06a80-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06a80-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06a80-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06a80-111">Permission type</span></span>|<span data-ttu-id="06a80-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06a80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06a80-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06a80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06a80-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06a80-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06a80-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06a80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06a80-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06a80-116">Not supported.</span></span>|
|<span data-ttu-id="06a80-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06a80-117">Application</span></span>|<span data-ttu-id="06a80-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06a80-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06a80-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06a80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="06a80-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06a80-120">Request headers</span></span>
|<span data-ttu-id="06a80-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06a80-121">Header</span></span>|<span data-ttu-id="06a80-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06a80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06a80-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06a80-123">Authorization</span></span>|<span data-ttu-id="06a80-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06a80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06a80-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06a80-125">Accept</span></span>|<span data-ttu-id="06a80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06a80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06a80-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06a80-127">Request body</span></span>
<span data-ttu-id="06a80-128">No corpo da solicitação, forneça uma representação JSON do objeto win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="06a80-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="06a80-129">A tabela a seguir mostra as propriedades que são necessárias ao criar win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="06a80-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="06a80-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06a80-130">Property</span></span>|<span data-ttu-id="06a80-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06a80-131">Type</span></span>|<span data-ttu-id="06a80-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06a80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06a80-133">id</span><span class="sxs-lookup"><span data-stu-id="06a80-133">id</span></span>|<span data-ttu-id="06a80-134">String</span><span class="sxs-lookup"><span data-stu-id="06a80-134">String</span></span>|<span data-ttu-id="06a80-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06a80-135">Key of the entity.</span></span> <span data-ttu-id="06a80-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-137">displayName</span><span class="sxs-lookup"><span data-stu-id="06a80-137">displayName</span></span>|<span data-ttu-id="06a80-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-138">String</span></span>|<span data-ttu-id="06a80-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="06a80-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="06a80-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-141">descrição</span><span class="sxs-lookup"><span data-stu-id="06a80-141">description</span></span>|<span data-ttu-id="06a80-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-142">String</span></span>|<span data-ttu-id="06a80-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-143">The description of the app.</span></span> <span data-ttu-id="06a80-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-145">publicador</span><span class="sxs-lookup"><span data-stu-id="06a80-145">publisher</span></span>|<span data-ttu-id="06a80-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-146">String</span></span>|<span data-ttu-id="06a80-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-147">The publisher of the app.</span></span> <span data-ttu-id="06a80-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="06a80-149">largeIcon</span></span>|[<span data-ttu-id="06a80-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="06a80-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="06a80-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="06a80-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="06a80-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06a80-153">createdDateTime</span></span>|<span data-ttu-id="06a80-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06a80-154">DateTimeOffset</span></span>|<span data-ttu-id="06a80-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-155">The date and time the app was created.</span></span> <span data-ttu-id="06a80-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06a80-157">lastModifiedDateTime</span></span>|<span data-ttu-id="06a80-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06a80-158">DateTimeOffset</span></span>|<span data-ttu-id="06a80-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="06a80-159">The date and time the app was last modified.</span></span> <span data-ttu-id="06a80-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="06a80-161">isFeatured</span></span>|<span data-ttu-id="06a80-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="06a80-162">Boolean</span></span>|<span data-ttu-id="06a80-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="06a80-164">privacyInformationUrl</span></span>|<span data-ttu-id="06a80-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-165">String</span></span>|<span data-ttu-id="06a80-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="06a80-166">The privacy statement Url.</span></span> <span data-ttu-id="06a80-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="06a80-168">informationUrl</span></span>|<span data-ttu-id="06a80-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-169">String</span></span>|<span data-ttu-id="06a80-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="06a80-170">The more information Url.</span></span> <span data-ttu-id="06a80-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-172">owner</span><span class="sxs-lookup"><span data-stu-id="06a80-172">owner</span></span>|<span data-ttu-id="06a80-173">String</span><span class="sxs-lookup"><span data-stu-id="06a80-173">String</span></span>|<span data-ttu-id="06a80-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="06a80-174">The owner of the app.</span></span> <span data-ttu-id="06a80-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-176">developer</span><span class="sxs-lookup"><span data-stu-id="06a80-176">developer</span></span>|<span data-ttu-id="06a80-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-177">String</span></span>|<span data-ttu-id="06a80-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-178">The developer of the app.</span></span> <span data-ttu-id="06a80-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-180">notes</span><span class="sxs-lookup"><span data-stu-id="06a80-180">notes</span></span>|<span data-ttu-id="06a80-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-181">String</span></span>|<span data-ttu-id="06a80-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-182">Notes for the app.</span></span> <span data-ttu-id="06a80-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="06a80-184">uploadState</span></span>|<span data-ttu-id="06a80-185">Int32</span><span class="sxs-lookup"><span data-stu-id="06a80-185">Int32</span></span>|<span data-ttu-id="06a80-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="06a80-186">The upload state.</span></span> <span data-ttu-id="06a80-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="06a80-188">publishingState</span></span>|[<span data-ttu-id="06a80-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="06a80-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="06a80-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-190">The publishing state for the app.</span></span> <span data-ttu-id="06a80-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="06a80-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="06a80-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="06a80-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="06a80-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="06a80-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="06a80-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="06a80-194">isAssigned</span></span>|<span data-ttu-id="06a80-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="06a80-195">Boolean</span></span>|<span data-ttu-id="06a80-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="06a80-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="06a80-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06a80-198">roleScopeTagIds</span></span>|<span data-ttu-id="06a80-199">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-199">String collection</span></span>|<span data-ttu-id="06a80-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="06a80-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="06a80-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="06a80-202">dependentAppCount</span></span>|<span data-ttu-id="06a80-203">Int32</span><span class="sxs-lookup"><span data-stu-id="06a80-203">Int32</span></span>|<span data-ttu-id="06a80-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="06a80-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="06a80-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="06a80-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="06a80-206">committedContentVersion</span></span>|<span data-ttu-id="06a80-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-207">String</span></span>|<span data-ttu-id="06a80-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="06a80-208">The internal committed content version.</span></span> <span data-ttu-id="06a80-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06a80-210">fileName</span><span class="sxs-lookup"><span data-stu-id="06a80-210">fileName</span></span>|<span data-ttu-id="06a80-211">String</span><span class="sxs-lookup"><span data-stu-id="06a80-211">String</span></span>|<span data-ttu-id="06a80-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="06a80-212">The name of the main Lob application file.</span></span> <span data-ttu-id="06a80-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06a80-214">size</span><span class="sxs-lookup"><span data-stu-id="06a80-214">size</span></span>|<span data-ttu-id="06a80-215">Int64</span><span class="sxs-lookup"><span data-stu-id="06a80-215">Int64</span></span>|<span data-ttu-id="06a80-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="06a80-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="06a80-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06a80-218">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="06a80-218">installCommandLine</span></span>|<span data-ttu-id="06a80-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-219">String</span></span>|<span data-ttu-id="06a80-220">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="06a80-220">The command line to install this app</span></span>|
|<span data-ttu-id="06a80-221">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="06a80-221">uninstallCommandLine</span></span>|<span data-ttu-id="06a80-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-222">String</span></span>|<span data-ttu-id="06a80-223">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="06a80-223">The command line to uninstall this app</span></span>|
|<span data-ttu-id="06a80-224">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="06a80-224">applicableArchitectures</span></span>|[<span data-ttu-id="06a80-225">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="06a80-225">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="06a80-226">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="06a80-226">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="06a80-227">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="06a80-227">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="06a80-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="06a80-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="06a80-229">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="06a80-229">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="06a80-230">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="06a80-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="06a80-231">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="06a80-231">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="06a80-232">Int32</span><span class="sxs-lookup"><span data-stu-id="06a80-232">Int32</span></span>|<span data-ttu-id="06a80-233">O valor para o espaço livre mínimo em disco necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-233">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="06a80-234">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="06a80-234">minimumMemoryInMB</span></span>|<span data-ttu-id="06a80-235">Int32</span><span class="sxs-lookup"><span data-stu-id="06a80-235">Int32</span></span>|<span data-ttu-id="06a80-236">O valor da memória física mínima exigida para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-236">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="06a80-237">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="06a80-237">minimumNumberOfProcessors</span></span>|<span data-ttu-id="06a80-238">Int32</span><span class="sxs-lookup"><span data-stu-id="06a80-238">Int32</span></span>|<span data-ttu-id="06a80-239">O valor para o número mínimo de processadores necessários para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-239">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="06a80-240">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="06a80-240">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="06a80-241">Int32</span><span class="sxs-lookup"><span data-stu-id="06a80-241">Int32</span></span>|<span data-ttu-id="06a80-242">O valor para a velocidade de CPU mínima necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-242">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="06a80-243">detectionRules</span><span class="sxs-lookup"><span data-stu-id="06a80-243">detectionRules</span></span>|<span data-ttu-id="06a80-244">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="06a80-245">As regras de detecção para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="06a80-245">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="06a80-246">requirementRules</span><span class="sxs-lookup"><span data-stu-id="06a80-246">requirementRules</span></span>|<span data-ttu-id="06a80-247">coleção [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="06a80-248">As regras de requisito para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="06a80-248">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="06a80-249">regras</span><span class="sxs-lookup"><span data-stu-id="06a80-249">rules</span></span>|<span data-ttu-id="06a80-250">coleção [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-250">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="06a80-251">As regras de detecção e requisitos para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-251">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="06a80-252">installExperience</span><span class="sxs-lookup"><span data-stu-id="06a80-252">installExperience</span></span>|[<span data-ttu-id="06a80-253">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="06a80-253">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="06a80-254">A experiência de instalação para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a80-254">The install experience for this app.</span></span>|
|<span data-ttu-id="06a80-255">returnCodes</span><span class="sxs-lookup"><span data-stu-id="06a80-255">returnCodes</span></span>|<span data-ttu-id="06a80-256">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="06a80-256">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="06a80-257">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="06a80-257">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="06a80-258">msiInformation</span><span class="sxs-lookup"><span data-stu-id="06a80-258">msiInformation</span></span>|[<span data-ttu-id="06a80-259">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="06a80-259">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="06a80-260">Os detalhes do MSI, se este aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="06a80-260">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="06a80-261">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="06a80-261">setupFilePath</span></span>|<span data-ttu-id="06a80-262">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-262">String</span></span>|<span data-ttu-id="06a80-263">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="06a80-263">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="06a80-264">installLanguage</span><span class="sxs-lookup"><span data-stu-id="06a80-264">installLanguage</span></span>|<span data-ttu-id="06a80-265">String</span><span class="sxs-lookup"><span data-stu-id="06a80-265">String</span></span>|<span data-ttu-id="06a80-266">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="06a80-266">Not yet documented</span></span>|
|<span data-ttu-id="06a80-267">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="06a80-267">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="06a80-268">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06a80-268">String</span></span>|<span data-ttu-id="06a80-269">O valor da versão mínima com suporte do Windows.</span><span class="sxs-lookup"><span data-stu-id="06a80-269">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="06a80-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a80-270">Response</span></span>
<span data-ttu-id="06a80-271">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06a80-271">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06a80-272">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06a80-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="06a80-273">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06a80-273">Request</span></span>
<span data-ttu-id="06a80-274">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06a80-274">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 3304

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
  "installLanguage": "Install Language value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```

### <a name="response"></a><span data-ttu-id="06a80-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a80-275">Response</span></span>
<span data-ttu-id="06a80-276">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="06a80-276">Here is an example of the response.</span></span> <span data-ttu-id="06a80-277">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="06a80-277">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="06a80-278">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="06a80-278">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3476

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
  "installLanguage": "Install Language value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```



