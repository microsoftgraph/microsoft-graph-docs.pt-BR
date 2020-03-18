---
title: Criar win32LobApp
description: Criar um novo objeto win32LobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52d7affd9eb1159320787c101fef6bfbaf74ec4d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760988"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="3733a-103">Criar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="3733a-103">Create win32LobApp</span></span>

> <span data-ttu-id="3733a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3733a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3733a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3733a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3733a-106">Criar um novo objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3733a-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3733a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3733a-107">Prerequisites</span></span>
<span data-ttu-id="3733a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3733a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3733a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3733a-110">Permission type</span></span>|<span data-ttu-id="3733a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3733a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3733a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3733a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3733a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3733a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3733a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3733a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3733a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3733a-115">Not supported.</span></span>|
|<span data-ttu-id="3733a-116">Application</span><span class="sxs-lookup"><span data-stu-id="3733a-116">Application</span></span>|<span data-ttu-id="3733a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3733a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3733a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3733a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3733a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3733a-119">Request headers</span></span>
|<span data-ttu-id="3733a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3733a-120">Header</span></span>|<span data-ttu-id="3733a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3733a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3733a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3733a-122">Authorization</span></span>|<span data-ttu-id="3733a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3733a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3733a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3733a-124">Accept</span></span>|<span data-ttu-id="3733a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3733a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3733a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3733a-126">Request body</span></span>
<span data-ttu-id="3733a-127">No corpo da solicitação, forneça uma representação JSON do objeto win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="3733a-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="3733a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="3733a-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="3733a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3733a-129">Property</span></span>|<span data-ttu-id="3733a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3733a-130">Type</span></span>|<span data-ttu-id="3733a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3733a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3733a-132">id</span><span class="sxs-lookup"><span data-stu-id="3733a-132">id</span></span>|<span data-ttu-id="3733a-133">String</span><span class="sxs-lookup"><span data-stu-id="3733a-133">String</span></span>|<span data-ttu-id="3733a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3733a-134">Key of the entity.</span></span> <span data-ttu-id="3733a-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3733a-136">displayName</span></span>|<span data-ttu-id="3733a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3733a-137">String</span></span>|<span data-ttu-id="3733a-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3733a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3733a-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-140">description</span><span class="sxs-lookup"><span data-stu-id="3733a-140">description</span></span>|<span data-ttu-id="3733a-141">String</span><span class="sxs-lookup"><span data-stu-id="3733a-141">String</span></span>|<span data-ttu-id="3733a-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-142">The description of the app.</span></span> <span data-ttu-id="3733a-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-144">publicador</span><span class="sxs-lookup"><span data-stu-id="3733a-144">publisher</span></span>|<span data-ttu-id="3733a-145">String</span><span class="sxs-lookup"><span data-stu-id="3733a-145">String</span></span>|<span data-ttu-id="3733a-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-146">The publisher of the app.</span></span> <span data-ttu-id="3733a-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3733a-148">largeIcon</span></span>|[<span data-ttu-id="3733a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3733a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3733a-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3733a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3733a-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3733a-152">createdDateTime</span></span>|<span data-ttu-id="3733a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3733a-153">DateTimeOffset</span></span>|<span data-ttu-id="3733a-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-154">The date and time the app was created.</span></span> <span data-ttu-id="3733a-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3733a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3733a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3733a-157">DateTimeOffset</span></span>|<span data-ttu-id="3733a-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3733a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3733a-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3733a-160">isFeatured</span></span>|<span data-ttu-id="3733a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3733a-161">Boolean</span></span>|<span data-ttu-id="3733a-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3733a-163">privacyInformationUrl</span></span>|<span data-ttu-id="3733a-164">String</span><span class="sxs-lookup"><span data-stu-id="3733a-164">String</span></span>|<span data-ttu-id="3733a-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3733a-165">The privacy statement Url.</span></span> <span data-ttu-id="3733a-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3733a-167">informationUrl</span></span>|<span data-ttu-id="3733a-168">String</span><span class="sxs-lookup"><span data-stu-id="3733a-168">String</span></span>|<span data-ttu-id="3733a-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3733a-169">The more information Url.</span></span> <span data-ttu-id="3733a-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-171">owner</span><span class="sxs-lookup"><span data-stu-id="3733a-171">owner</span></span>|<span data-ttu-id="3733a-172">String</span><span class="sxs-lookup"><span data-stu-id="3733a-172">String</span></span>|<span data-ttu-id="3733a-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3733a-173">The owner of the app.</span></span> <span data-ttu-id="3733a-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-175">developer</span><span class="sxs-lookup"><span data-stu-id="3733a-175">developer</span></span>|<span data-ttu-id="3733a-176">String</span><span class="sxs-lookup"><span data-stu-id="3733a-176">String</span></span>|<span data-ttu-id="3733a-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-177">The developer of the app.</span></span> <span data-ttu-id="3733a-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-179">notes</span><span class="sxs-lookup"><span data-stu-id="3733a-179">notes</span></span>|<span data-ttu-id="3733a-180">String</span><span class="sxs-lookup"><span data-stu-id="3733a-180">String</span></span>|<span data-ttu-id="3733a-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-181">Notes for the app.</span></span> <span data-ttu-id="3733a-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3733a-183">uploadState</span></span>|<span data-ttu-id="3733a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3733a-184">Int32</span></span>|<span data-ttu-id="3733a-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="3733a-185">The upload state.</span></span> <span data-ttu-id="3733a-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3733a-187">publishingState</span></span>|[<span data-ttu-id="3733a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3733a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3733a-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-189">The publishing state for the app.</span></span> <span data-ttu-id="3733a-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3733a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3733a-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3733a-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="3733a-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3733a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3733a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3733a-193">isAssigned</span></span>|<span data-ttu-id="3733a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3733a-194">Boolean</span></span>|<span data-ttu-id="3733a-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="3733a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3733a-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3733a-197">roleScopeTagIds</span></span>|<span data-ttu-id="3733a-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3733a-198">String collection</span></span>|<span data-ttu-id="3733a-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="3733a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3733a-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="3733a-201">dependentAppCount</span></span>|<span data-ttu-id="3733a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="3733a-202">Int32</span></span>|<span data-ttu-id="3733a-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="3733a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3733a-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3733a-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3733a-205">committedContentVersion</span></span>|<span data-ttu-id="3733a-206">String</span><span class="sxs-lookup"><span data-stu-id="3733a-206">String</span></span>|<span data-ttu-id="3733a-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="3733a-207">The internal committed content version.</span></span> <span data-ttu-id="3733a-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3733a-209">fileName</span><span class="sxs-lookup"><span data-stu-id="3733a-209">fileName</span></span>|<span data-ttu-id="3733a-210">String</span><span class="sxs-lookup"><span data-stu-id="3733a-210">String</span></span>|<span data-ttu-id="3733a-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="3733a-211">The name of the main Lob application file.</span></span> <span data-ttu-id="3733a-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3733a-213">size</span><span class="sxs-lookup"><span data-stu-id="3733a-213">size</span></span>|<span data-ttu-id="3733a-214">Int64</span><span class="sxs-lookup"><span data-stu-id="3733a-214">Int64</span></span>|<span data-ttu-id="3733a-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="3733a-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="3733a-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3733a-217">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="3733a-217">installCommandLine</span></span>|<span data-ttu-id="3733a-218">String</span><span class="sxs-lookup"><span data-stu-id="3733a-218">String</span></span>|<span data-ttu-id="3733a-219">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="3733a-219">The command line to install this app</span></span>|
|<span data-ttu-id="3733a-220">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="3733a-220">uninstallCommandLine</span></span>|<span data-ttu-id="3733a-221">String</span><span class="sxs-lookup"><span data-stu-id="3733a-221">String</span></span>|<span data-ttu-id="3733a-222">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="3733a-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="3733a-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="3733a-223">applicableArchitectures</span></span>|[<span data-ttu-id="3733a-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="3733a-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="3733a-225">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="3733a-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="3733a-226">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="3733a-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="3733a-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3733a-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3733a-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3733a-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="3733a-229">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="3733a-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3733a-230">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="3733a-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="3733a-231">Int32</span><span class="sxs-lookup"><span data-stu-id="3733a-231">Int32</span></span>|<span data-ttu-id="3733a-232">O valor para o espaço livre mínimo em disco necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="3733a-233">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="3733a-233">minimumMemoryInMB</span></span>|<span data-ttu-id="3733a-234">Int32</span><span class="sxs-lookup"><span data-stu-id="3733a-234">Int32</span></span>|<span data-ttu-id="3733a-235">O valor da memória física mínima exigida para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="3733a-236">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="3733a-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="3733a-237">Int32</span><span class="sxs-lookup"><span data-stu-id="3733a-237">Int32</span></span>|<span data-ttu-id="3733a-238">O valor para o número mínimo de processadores necessários para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="3733a-239">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="3733a-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="3733a-240">Int32</span><span class="sxs-lookup"><span data-stu-id="3733a-240">Int32</span></span>|<span data-ttu-id="3733a-241">O valor para a velocidade de CPU mínima necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="3733a-242">detectionRules</span><span class="sxs-lookup"><span data-stu-id="3733a-242">detectionRules</span></span>|<span data-ttu-id="3733a-243">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="3733a-244">As regras de detecção para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="3733a-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3733a-245">requirementRules</span><span class="sxs-lookup"><span data-stu-id="3733a-245">requirementRules</span></span>|<span data-ttu-id="3733a-246">coleção [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="3733a-247">As regras de requisito para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="3733a-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3733a-248">installExperience</span><span class="sxs-lookup"><span data-stu-id="3733a-248">installExperience</span></span>|[<span data-ttu-id="3733a-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="3733a-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="3733a-250">A experiência de instalação para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3733a-250">The install experience for this app.</span></span>|
|<span data-ttu-id="3733a-251">returnCodes</span><span class="sxs-lookup"><span data-stu-id="3733a-251">returnCodes</span></span>|<span data-ttu-id="3733a-252">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="3733a-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="3733a-253">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="3733a-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="3733a-254">msiInformation</span><span class="sxs-lookup"><span data-stu-id="3733a-254">msiInformation</span></span>|[<span data-ttu-id="3733a-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="3733a-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="3733a-256">Os detalhes do MSI, se este aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="3733a-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="3733a-257">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="3733a-257">setupFilePath</span></span>|<span data-ttu-id="3733a-258">String</span><span class="sxs-lookup"><span data-stu-id="3733a-258">String</span></span>|<span data-ttu-id="3733a-259">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="3733a-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="3733a-260">installLanguage</span><span class="sxs-lookup"><span data-stu-id="3733a-260">installLanguage</span></span>|<span data-ttu-id="3733a-261">String</span><span class="sxs-lookup"><span data-stu-id="3733a-261">String</span></span>|<span data-ttu-id="3733a-262">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3733a-262">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3733a-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="3733a-263">Response</span></span>
<span data-ttu-id="3733a-264">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3733a-264">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3733a-265">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3733a-265">Example</span></span>

### <a name="request"></a><span data-ttu-id="3733a-266">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3733a-266">Request</span></span>
<span data-ttu-id="3733a-267">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3733a-267">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2865

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

### <a name="response"></a><span data-ttu-id="3733a-268">Resposta</span><span class="sxs-lookup"><span data-stu-id="3733a-268">Response</span></span>
<span data-ttu-id="3733a-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3733a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3037

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




