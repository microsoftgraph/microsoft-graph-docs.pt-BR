---
title: Atualizar win32LobApp
description: Atualiza as propriedades de um objeto win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0b4f57f494722083175a2adcfdb25aec48a9886
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973268"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="06ede-103">Atualizar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="06ede-103">Update win32LobApp</span></span>

> <span data-ttu-id="06ede-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06ede-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06ede-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06ede-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06ede-106">Atualiza as propriedades de um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="06ede-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06ede-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06ede-107">Prerequisites</span></span>
<span data-ttu-id="06ede-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06ede-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06ede-110">Permission type</span></span>|<span data-ttu-id="06ede-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06ede-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06ede-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06ede-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06ede-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ede-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06ede-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06ede-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06ede-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06ede-115">Not supported.</span></span>|
|<span data-ttu-id="06ede-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06ede-116">Application</span></span>|<span data-ttu-id="06ede-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06ede-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06ede-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06ede-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="06ede-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06ede-119">Request headers</span></span>
|<span data-ttu-id="06ede-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06ede-120">Header</span></span>|<span data-ttu-id="06ede-121">Valor</span><span class="sxs-lookup"><span data-stu-id="06ede-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06ede-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="06ede-122">Authorization</span></span>|<span data-ttu-id="06ede-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06ede-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06ede-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06ede-124">Accept</span></span>|<span data-ttu-id="06ede-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06ede-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06ede-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06ede-126">Request body</span></span>
<span data-ttu-id="06ede-127">No corpo da solicitação, forneça uma representação JSON do objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="06ede-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="06ede-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="06ede-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="06ede-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06ede-129">Property</span></span>|<span data-ttu-id="06ede-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="06ede-130">Type</span></span>|<span data-ttu-id="06ede-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="06ede-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ede-132">id</span><span class="sxs-lookup"><span data-stu-id="06ede-132">id</span></span>|<span data-ttu-id="06ede-133">String</span><span class="sxs-lookup"><span data-stu-id="06ede-133">String</span></span>|<span data-ttu-id="06ede-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06ede-134">Key of the entity.</span></span> <span data-ttu-id="06ede-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-136">displayName</span><span class="sxs-lookup"><span data-stu-id="06ede-136">displayName</span></span>|<span data-ttu-id="06ede-137">String</span><span class="sxs-lookup"><span data-stu-id="06ede-137">String</span></span>|<span data-ttu-id="06ede-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="06ede-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="06ede-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-140">descrição</span><span class="sxs-lookup"><span data-stu-id="06ede-140">description</span></span>|<span data-ttu-id="06ede-141">String</span><span class="sxs-lookup"><span data-stu-id="06ede-141">String</span></span>|<span data-ttu-id="06ede-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-142">The description of the app.</span></span> <span data-ttu-id="06ede-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-144">publicador</span><span class="sxs-lookup"><span data-stu-id="06ede-144">publisher</span></span>|<span data-ttu-id="06ede-145">String</span><span class="sxs-lookup"><span data-stu-id="06ede-145">String</span></span>|<span data-ttu-id="06ede-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-146">The publisher of the app.</span></span> <span data-ttu-id="06ede-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="06ede-148">largeIcon</span></span>|[<span data-ttu-id="06ede-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="06ede-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="06ede-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="06ede-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="06ede-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06ede-152">createdDateTime</span></span>|<span data-ttu-id="06ede-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ede-153">DateTimeOffset</span></span>|<span data-ttu-id="06ede-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-154">The date and time the app was created.</span></span> <span data-ttu-id="06ede-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06ede-156">lastModifiedDateTime</span></span>|<span data-ttu-id="06ede-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ede-157">DateTimeOffset</span></span>|<span data-ttu-id="06ede-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="06ede-158">The date and time the app was last modified.</span></span> <span data-ttu-id="06ede-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="06ede-160">isFeatured</span></span>|<span data-ttu-id="06ede-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="06ede-161">Boolean</span></span>|<span data-ttu-id="06ede-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="06ede-163">privacyInformationUrl</span></span>|<span data-ttu-id="06ede-164">String</span><span class="sxs-lookup"><span data-stu-id="06ede-164">String</span></span>|<span data-ttu-id="06ede-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="06ede-165">The privacy statement Url.</span></span> <span data-ttu-id="06ede-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="06ede-167">informationUrl</span></span>|<span data-ttu-id="06ede-168">String</span><span class="sxs-lookup"><span data-stu-id="06ede-168">String</span></span>|<span data-ttu-id="06ede-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="06ede-169">The more information Url.</span></span> <span data-ttu-id="06ede-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-171">owner</span><span class="sxs-lookup"><span data-stu-id="06ede-171">owner</span></span>|<span data-ttu-id="06ede-172">String</span><span class="sxs-lookup"><span data-stu-id="06ede-172">String</span></span>|<span data-ttu-id="06ede-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="06ede-173">The owner of the app.</span></span> <span data-ttu-id="06ede-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-175">developer</span><span class="sxs-lookup"><span data-stu-id="06ede-175">developer</span></span>|<span data-ttu-id="06ede-176">String</span><span class="sxs-lookup"><span data-stu-id="06ede-176">String</span></span>|<span data-ttu-id="06ede-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-177">The developer of the app.</span></span> <span data-ttu-id="06ede-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-179">notes</span><span class="sxs-lookup"><span data-stu-id="06ede-179">notes</span></span>|<span data-ttu-id="06ede-180">String</span><span class="sxs-lookup"><span data-stu-id="06ede-180">String</span></span>|<span data-ttu-id="06ede-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-181">Notes for the app.</span></span> <span data-ttu-id="06ede-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="06ede-183">uploadState</span></span>|<span data-ttu-id="06ede-184">Int32</span><span class="sxs-lookup"><span data-stu-id="06ede-184">Int32</span></span>|<span data-ttu-id="06ede-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="06ede-185">The upload state.</span></span> <span data-ttu-id="06ede-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="06ede-187">publishingState</span></span>|[<span data-ttu-id="06ede-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="06ede-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="06ede-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-189">The publishing state for the app.</span></span> <span data-ttu-id="06ede-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="06ede-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="06ede-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="06ede-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="06ede-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="06ede-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="06ede-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="06ede-193">isAssigned</span></span>|<span data-ttu-id="06ede-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="06ede-194">Boolean</span></span>|<span data-ttu-id="06ede-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="06ede-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="06ede-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06ede-197">roleScopeTagIds</span></span>|<span data-ttu-id="06ede-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="06ede-198">String collection</span></span>|<span data-ttu-id="06ede-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="06ede-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="06ede-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="06ede-201">dependentAppCount</span></span>|<span data-ttu-id="06ede-202">Int32</span><span class="sxs-lookup"><span data-stu-id="06ede-202">Int32</span></span>|<span data-ttu-id="06ede-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="06ede-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="06ede-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06ede-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="06ede-205">committedContentVersion</span></span>|<span data-ttu-id="06ede-206">String</span><span class="sxs-lookup"><span data-stu-id="06ede-206">String</span></span>|<span data-ttu-id="06ede-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="06ede-207">The internal committed content version.</span></span> <span data-ttu-id="06ede-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06ede-209">fileName</span><span class="sxs-lookup"><span data-stu-id="06ede-209">fileName</span></span>|<span data-ttu-id="06ede-210">String</span><span class="sxs-lookup"><span data-stu-id="06ede-210">String</span></span>|<span data-ttu-id="06ede-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="06ede-211">The name of the main Lob application file.</span></span> <span data-ttu-id="06ede-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06ede-213">size</span><span class="sxs-lookup"><span data-stu-id="06ede-213">size</span></span>|<span data-ttu-id="06ede-214">Int64</span><span class="sxs-lookup"><span data-stu-id="06ede-214">Int64</span></span>|<span data-ttu-id="06ede-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="06ede-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="06ede-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06ede-217">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="06ede-217">installCommandLine</span></span>|<span data-ttu-id="06ede-218">String</span><span class="sxs-lookup"><span data-stu-id="06ede-218">String</span></span>|<span data-ttu-id="06ede-219">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="06ede-219">The command line to install this app</span></span>|
|<span data-ttu-id="06ede-220">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="06ede-220">uninstallCommandLine</span></span>|<span data-ttu-id="06ede-221">String</span><span class="sxs-lookup"><span data-stu-id="06ede-221">String</span></span>|<span data-ttu-id="06ede-222">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="06ede-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="06ede-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="06ede-223">applicableArchitectures</span></span>|[<span data-ttu-id="06ede-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="06ede-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="06ede-225">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="06ede-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="06ede-226">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="06ede-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="06ede-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="06ede-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="06ede-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="06ede-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="06ede-229">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="06ede-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="06ede-230">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="06ede-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="06ede-231">Int32</span><span class="sxs-lookup"><span data-stu-id="06ede-231">Int32</span></span>|<span data-ttu-id="06ede-232">O valor para o espaço livre mínimo em disco necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="06ede-233">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="06ede-233">minimumMemoryInMB</span></span>|<span data-ttu-id="06ede-234">Int32</span><span class="sxs-lookup"><span data-stu-id="06ede-234">Int32</span></span>|<span data-ttu-id="06ede-235">O valor da memória física mínima exigida para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="06ede-236">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="06ede-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="06ede-237">Int32</span><span class="sxs-lookup"><span data-stu-id="06ede-237">Int32</span></span>|<span data-ttu-id="06ede-238">O valor para o número mínimo de processadores necessários para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="06ede-239">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="06ede-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="06ede-240">Int32</span><span class="sxs-lookup"><span data-stu-id="06ede-240">Int32</span></span>|<span data-ttu-id="06ede-241">O valor para a velocidade de CPU mínima necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="06ede-242">detectionRules</span><span class="sxs-lookup"><span data-stu-id="06ede-242">detectionRules</span></span>|<span data-ttu-id="06ede-243">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="06ede-244">As regras de detecção para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="06ede-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="06ede-245">requirementRules</span><span class="sxs-lookup"><span data-stu-id="06ede-245">requirementRules</span></span>|<span data-ttu-id="06ede-246">coleção [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="06ede-247">As regras de requisito para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="06ede-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="06ede-248">installExperience</span><span class="sxs-lookup"><span data-stu-id="06ede-248">installExperience</span></span>|[<span data-ttu-id="06ede-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="06ede-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="06ede-250">A experiência de instalação para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06ede-250">The install experience for this app.</span></span>|
|<span data-ttu-id="06ede-251">returnCodes</span><span class="sxs-lookup"><span data-stu-id="06ede-251">returnCodes</span></span>|<span data-ttu-id="06ede-252">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="06ede-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="06ede-253">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="06ede-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="06ede-254">msiInformation</span><span class="sxs-lookup"><span data-stu-id="06ede-254">msiInformation</span></span>|[<span data-ttu-id="06ede-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="06ede-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="06ede-256">Os detalhes do MSI, se este aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="06ede-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="06ede-257">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="06ede-257">setupFilePath</span></span>|<span data-ttu-id="06ede-258">String</span><span class="sxs-lookup"><span data-stu-id="06ede-258">String</span></span>|<span data-ttu-id="06ede-259">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="06ede-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="06ede-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ede-260">Response</span></span>
<span data-ttu-id="06ede-261">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06ede-261">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06ede-262">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06ede-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="06ede-263">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06ede-263">Request</span></span>
<span data-ttu-id="06ede-264">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06ede-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2778

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
    "runAsAccount": "user"
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

### <a name="response"></a><span data-ttu-id="06ede-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ede-265">Response</span></span>
<span data-ttu-id="06ede-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06ede-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2950

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
    "runAsAccount": "user"
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





