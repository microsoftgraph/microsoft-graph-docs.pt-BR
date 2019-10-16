---
title: Atualizar win32LobApp
description: Atualiza as propriedades de um objeto win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f149b3f2867309718d2c4eefb194ad787951d88
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535104"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="de880-103">Atualizar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="de880-103">Update win32LobApp</span></span>

> <span data-ttu-id="de880-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de880-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de880-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de880-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de880-106">Atualiza as propriedades de um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="de880-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de880-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de880-107">Prerequisites</span></span>
<span data-ttu-id="de880-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de880-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de880-110">Permission type</span></span>|<span data-ttu-id="de880-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de880-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de880-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de880-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de880-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de880-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de880-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de880-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de880-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de880-115">Not supported.</span></span>|
|<span data-ttu-id="de880-116">Application</span><span class="sxs-lookup"><span data-stu-id="de880-116">Application</span></span>|<span data-ttu-id="de880-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de880-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de880-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de880-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="de880-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de880-119">Request headers</span></span>
|<span data-ttu-id="de880-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de880-120">Header</span></span>|<span data-ttu-id="de880-121">Valor</span><span class="sxs-lookup"><span data-stu-id="de880-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de880-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="de880-122">Authorization</span></span>|<span data-ttu-id="de880-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de880-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de880-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de880-124">Accept</span></span>|<span data-ttu-id="de880-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de880-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de880-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de880-126">Request body</span></span>
<span data-ttu-id="de880-127">No corpo da solicitação, forneça uma representação JSON do objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="de880-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="de880-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="de880-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="de880-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de880-129">Property</span></span>|<span data-ttu-id="de880-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="de880-130">Type</span></span>|<span data-ttu-id="de880-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="de880-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de880-132">id</span><span class="sxs-lookup"><span data-stu-id="de880-132">id</span></span>|<span data-ttu-id="de880-133">String</span><span class="sxs-lookup"><span data-stu-id="de880-133">String</span></span>|<span data-ttu-id="de880-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de880-134">Key of the entity.</span></span> <span data-ttu-id="de880-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-136">displayName</span><span class="sxs-lookup"><span data-stu-id="de880-136">displayName</span></span>|<span data-ttu-id="de880-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-137">String</span></span>|<span data-ttu-id="de880-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="de880-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="de880-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-140">description</span><span class="sxs-lookup"><span data-stu-id="de880-140">description</span></span>|<span data-ttu-id="de880-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-141">String</span></span>|<span data-ttu-id="de880-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-142">The description of the app.</span></span> <span data-ttu-id="de880-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-144">publicador</span><span class="sxs-lookup"><span data-stu-id="de880-144">publisher</span></span>|<span data-ttu-id="de880-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-145">String</span></span>|<span data-ttu-id="de880-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-146">The publisher of the app.</span></span> <span data-ttu-id="de880-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="de880-148">largeIcon</span></span>|[<span data-ttu-id="de880-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="de880-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="de880-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="de880-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="de880-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de880-152">createdDateTime</span></span>|<span data-ttu-id="de880-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de880-153">DateTimeOffset</span></span>|<span data-ttu-id="de880-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-154">The date and time the app was created.</span></span> <span data-ttu-id="de880-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de880-156">lastModifiedDateTime</span></span>|<span data-ttu-id="de880-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de880-157">DateTimeOffset</span></span>|<span data-ttu-id="de880-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="de880-158">The date and time the app was last modified.</span></span> <span data-ttu-id="de880-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="de880-160">isFeatured</span></span>|<span data-ttu-id="de880-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="de880-161">Boolean</span></span>|<span data-ttu-id="de880-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="de880-163">privacyInformationUrl</span></span>|<span data-ttu-id="de880-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-164">String</span></span>|<span data-ttu-id="de880-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="de880-165">The privacy statement Url.</span></span> <span data-ttu-id="de880-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="de880-167">informationUrl</span></span>|<span data-ttu-id="de880-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-168">String</span></span>|<span data-ttu-id="de880-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="de880-169">The more information Url.</span></span> <span data-ttu-id="de880-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-171">owner</span><span class="sxs-lookup"><span data-stu-id="de880-171">owner</span></span>|<span data-ttu-id="de880-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-172">String</span></span>|<span data-ttu-id="de880-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="de880-173">The owner of the app.</span></span> <span data-ttu-id="de880-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-175">developer</span><span class="sxs-lookup"><span data-stu-id="de880-175">developer</span></span>|<span data-ttu-id="de880-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-176">String</span></span>|<span data-ttu-id="de880-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-177">The developer of the app.</span></span> <span data-ttu-id="de880-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-179">notes</span><span class="sxs-lookup"><span data-stu-id="de880-179">notes</span></span>|<span data-ttu-id="de880-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-180">String</span></span>|<span data-ttu-id="de880-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-181">Notes for the app.</span></span> <span data-ttu-id="de880-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="de880-183">uploadState</span></span>|<span data-ttu-id="de880-184">Int32</span><span class="sxs-lookup"><span data-stu-id="de880-184">Int32</span></span>|<span data-ttu-id="de880-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="de880-185">The upload state.</span></span> <span data-ttu-id="de880-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="de880-187">publishingState</span></span>|[<span data-ttu-id="de880-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="de880-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="de880-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-189">The publishing state for the app.</span></span> <span data-ttu-id="de880-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="de880-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="de880-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de880-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="de880-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="de880-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="de880-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="de880-193">isAssigned</span></span>|<span data-ttu-id="de880-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="de880-194">Boolean</span></span>|<span data-ttu-id="de880-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="de880-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="de880-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de880-197">roleScopeTagIds</span></span>|<span data-ttu-id="de880-198">String collection</span><span class="sxs-lookup"><span data-stu-id="de880-198">String collection</span></span>|<span data-ttu-id="de880-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="de880-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="de880-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="de880-201">dependentAppCount</span></span>|<span data-ttu-id="de880-202">Int32</span><span class="sxs-lookup"><span data-stu-id="de880-202">Int32</span></span>|<span data-ttu-id="de880-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="de880-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="de880-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de880-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="de880-205">committedContentVersion</span></span>|<span data-ttu-id="de880-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-206">String</span></span>|<span data-ttu-id="de880-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="de880-207">The internal committed content version.</span></span> <span data-ttu-id="de880-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="de880-209">fileName</span><span class="sxs-lookup"><span data-stu-id="de880-209">fileName</span></span>|<span data-ttu-id="de880-210">String</span><span class="sxs-lookup"><span data-stu-id="de880-210">String</span></span>|<span data-ttu-id="de880-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="de880-211">The name of the main Lob application file.</span></span> <span data-ttu-id="de880-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="de880-213">size</span><span class="sxs-lookup"><span data-stu-id="de880-213">size</span></span>|<span data-ttu-id="de880-214">Int64</span><span class="sxs-lookup"><span data-stu-id="de880-214">Int64</span></span>|<span data-ttu-id="de880-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="de880-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="de880-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="de880-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="de880-217">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="de880-217">installCommandLine</span></span>|<span data-ttu-id="de880-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-218">String</span></span>|<span data-ttu-id="de880-219">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="de880-219">The command line to install this app</span></span>|
|<span data-ttu-id="de880-220">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="de880-220">uninstallCommandLine</span></span>|<span data-ttu-id="de880-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-221">String</span></span>|<span data-ttu-id="de880-222">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="de880-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="de880-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="de880-223">applicableArchitectures</span></span>|[<span data-ttu-id="de880-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="de880-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="de880-225">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="de880-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="de880-226">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="de880-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="de880-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="de880-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="de880-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="de880-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="de880-229">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="de880-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="de880-230">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="de880-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="de880-231">Int32</span><span class="sxs-lookup"><span data-stu-id="de880-231">Int32</span></span>|<span data-ttu-id="de880-232">O valor para o espaço livre mínimo em disco necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="de880-233">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="de880-233">minimumMemoryInMB</span></span>|<span data-ttu-id="de880-234">Int32</span><span class="sxs-lookup"><span data-stu-id="de880-234">Int32</span></span>|<span data-ttu-id="de880-235">O valor da memória física mínima exigida para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="de880-236">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="de880-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="de880-237">Int32</span><span class="sxs-lookup"><span data-stu-id="de880-237">Int32</span></span>|<span data-ttu-id="de880-238">O valor para o número mínimo de processadores necessários para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="de880-239">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="de880-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="de880-240">Int32</span><span class="sxs-lookup"><span data-stu-id="de880-240">Int32</span></span>|<span data-ttu-id="de880-241">O valor para a velocidade de CPU mínima necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="de880-242">detectionRules</span><span class="sxs-lookup"><span data-stu-id="de880-242">detectionRules</span></span>|<span data-ttu-id="de880-243">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="de880-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="de880-244">As regras de detecção para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="de880-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="de880-245">requirementRules</span><span class="sxs-lookup"><span data-stu-id="de880-245">requirementRules</span></span>|<span data-ttu-id="de880-246">coleção [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="de880-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="de880-247">As regras de requisito para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="de880-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="de880-248">installExperience</span><span class="sxs-lookup"><span data-stu-id="de880-248">installExperience</span></span>|[<span data-ttu-id="de880-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="de880-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="de880-250">A experiência de instalação para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de880-250">The install experience for this app.</span></span>|
|<span data-ttu-id="de880-251">returnCodes</span><span class="sxs-lookup"><span data-stu-id="de880-251">returnCodes</span></span>|<span data-ttu-id="de880-252">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="de880-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="de880-253">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="de880-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="de880-254">msiInformation</span><span class="sxs-lookup"><span data-stu-id="de880-254">msiInformation</span></span>|[<span data-ttu-id="de880-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="de880-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="de880-256">Os detalhes do MSI, se este aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="de880-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="de880-257">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="de880-257">setupFilePath</span></span>|<span data-ttu-id="de880-258">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de880-258">String</span></span>|<span data-ttu-id="de880-259">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="de880-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="de880-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="de880-260">Response</span></span>
<span data-ttu-id="de880-261">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de880-261">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de880-262">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de880-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="de880-263">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de880-263">Request</span></span>
<span data-ttu-id="de880-264">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de880-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2817

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
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="de880-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="de880-265">Response</span></span>
<span data-ttu-id="de880-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de880-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2989

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
  "setupFilePath": "Setup File Path value"
}
```






