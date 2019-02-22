---
title: Criar win32LobApp
description: Criar um novo objeto win32LobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89336782798f92a3626a8a46a0ab49cd8b765da3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168471"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="a1bdb-103">Criar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="a1bdb-103">Create win32LobApp</span></span>

> <span data-ttu-id="a1bdb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1bdb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1bdb-106">Criar um novo objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a1bdb-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1bdb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1bdb-107">Prerequisites</span></span>
<span data-ttu-id="a1bdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1bdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a1bdb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1bdb-110">Permission type</span></span>|<span data-ttu-id="a1bdb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1bdb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1bdb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1bdb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1bdb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1bdb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-115">Not supported.</span></span>|
|<span data-ttu-id="a1bdb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1bdb-116">Application</span></span>|<span data-ttu-id="a1bdb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1bdb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1bdb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a1bdb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1bdb-119">Request headers</span></span>
|<span data-ttu-id="a1bdb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1bdb-120">Header</span></span>|<span data-ttu-id="a1bdb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1bdb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1bdb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1bdb-122">Authorization</span></span>|<span data-ttu-id="a1bdb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1bdb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1bdb-124">Accept</span></span>|<span data-ttu-id="a1bdb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1bdb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1bdb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1bdb-126">Request body</span></span>
<span data-ttu-id="a1bdb-127">No corpo da solicitação, forneça uma representação JSON do objeto win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="a1bdb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="a1bdb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1bdb-129">Property</span></span>|<span data-ttu-id="a1bdb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1bdb-130">Type</span></span>|<span data-ttu-id="a1bdb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1bdb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1bdb-132">id</span><span class="sxs-lookup"><span data-stu-id="a1bdb-132">id</span></span>|<span data-ttu-id="a1bdb-133">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-133">String</span></span>|<span data-ttu-id="a1bdb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-134">Key of the entity.</span></span> <span data-ttu-id="a1bdb-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a1bdb-136">displayName</span></span>|<span data-ttu-id="a1bdb-137">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-137">String</span></span>|<span data-ttu-id="a1bdb-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a1bdb-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-140">description</span><span class="sxs-lookup"><span data-stu-id="a1bdb-140">description</span></span>|<span data-ttu-id="a1bdb-141">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-141">String</span></span>|<span data-ttu-id="a1bdb-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-142">The description of the app.</span></span> <span data-ttu-id="a1bdb-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a1bdb-144">publisher</span></span>|<span data-ttu-id="a1bdb-145">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-145">String</span></span>|<span data-ttu-id="a1bdb-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-146">The publisher of the app.</span></span> <span data-ttu-id="a1bdb-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a1bdb-148">largeIcon</span></span>|[<span data-ttu-id="a1bdb-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a1bdb-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a1bdb-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a1bdb-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1bdb-152">createdDateTime</span></span>|<span data-ttu-id="a1bdb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1bdb-153">DateTimeOffset</span></span>|<span data-ttu-id="a1bdb-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-154">The date and time the app was created.</span></span> <span data-ttu-id="a1bdb-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1bdb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a1bdb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1bdb-157">DateTimeOffset</span></span>|<span data-ttu-id="a1bdb-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a1bdb-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a1bdb-160">isFeatured</span></span>|<span data-ttu-id="a1bdb-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1bdb-161">Boolean</span></span>|<span data-ttu-id="a1bdb-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a1bdb-163">privacyInformationUrl</span></span>|<span data-ttu-id="a1bdb-164">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-164">String</span></span>|<span data-ttu-id="a1bdb-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-165">The privacy statement Url.</span></span> <span data-ttu-id="a1bdb-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a1bdb-167">informationUrl</span></span>|<span data-ttu-id="a1bdb-168">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-168">String</span></span>|<span data-ttu-id="a1bdb-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-169">The more information Url.</span></span> <span data-ttu-id="a1bdb-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-171">owner</span><span class="sxs-lookup"><span data-stu-id="a1bdb-171">owner</span></span>|<span data-ttu-id="a1bdb-172">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-172">String</span></span>|<span data-ttu-id="a1bdb-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-173">The owner of the app.</span></span> <span data-ttu-id="a1bdb-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-175">developer</span><span class="sxs-lookup"><span data-stu-id="a1bdb-175">developer</span></span>|<span data-ttu-id="a1bdb-176">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-176">String</span></span>|<span data-ttu-id="a1bdb-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-177">The developer of the app.</span></span> <span data-ttu-id="a1bdb-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-179">Observações</span><span class="sxs-lookup"><span data-stu-id="a1bdb-179">notes</span></span>|<span data-ttu-id="a1bdb-180">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-180">String</span></span>|<span data-ttu-id="a1bdb-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-181">Notes for the app.</span></span> <span data-ttu-id="a1bdb-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a1bdb-183">uploadState</span></span>|<span data-ttu-id="a1bdb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a1bdb-184">Int32</span></span>|<span data-ttu-id="a1bdb-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-185">The upload state.</span></span> <span data-ttu-id="a1bdb-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a1bdb-187">publishingState</span></span>|[<span data-ttu-id="a1bdb-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a1bdb-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a1bdb-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-189">The publishing state for the app.</span></span> <span data-ttu-id="a1bdb-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a1bdb-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1bdb-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a1bdb-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a1bdb-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a1bdb-193">isAssigned</span></span>|<span data-ttu-id="a1bdb-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1bdb-194">Boolean</span></span>|<span data-ttu-id="a1bdb-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a1bdb-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1bdb-197">roleScopeTagIds</span></span>|<span data-ttu-id="a1bdb-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1bdb-198">String collection</span></span>|<span data-ttu-id="a1bdb-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a1bdb-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a1bdb-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a1bdb-201">committedContentVersion</span></span>|<span data-ttu-id="a1bdb-202">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-202">String</span></span>|<span data-ttu-id="a1bdb-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-203">The internal committed content version.</span></span> <span data-ttu-id="a1bdb-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a1bdb-205">fileName</span><span class="sxs-lookup"><span data-stu-id="a1bdb-205">fileName</span></span>|<span data-ttu-id="a1bdb-206">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-206">String</span></span>|<span data-ttu-id="a1bdb-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-207">The name of the main Lob application file.</span></span> <span data-ttu-id="a1bdb-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a1bdb-209">size</span><span class="sxs-lookup"><span data-stu-id="a1bdb-209">size</span></span>|<span data-ttu-id="a1bdb-210">Int64</span><span class="sxs-lookup"><span data-stu-id="a1bdb-210">Int64</span></span>|<span data-ttu-id="a1bdb-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="a1bdb-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a1bdb-213">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="a1bdb-213">installCommandLine</span></span>|<span data-ttu-id="a1bdb-214">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-214">String</span></span>|<span data-ttu-id="a1bdb-215">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1bdb-215">The command line to install this app</span></span>|
|<span data-ttu-id="a1bdb-216">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="a1bdb-216">uninstallCommandLine</span></span>|<span data-ttu-id="a1bdb-217">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-217">String</span></span>|<span data-ttu-id="a1bdb-218">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1bdb-218">The command line to uninstall this app</span></span>|
|<span data-ttu-id="a1bdb-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="a1bdb-219">applicableArchitectures</span></span>|[<span data-ttu-id="a1bdb-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a1bdb-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a1bdb-221">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="a1bdb-222">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a1bdb-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a1bdb-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a1bdb-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a1bdb-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="a1bdb-225">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a1bdb-226">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="a1bdb-226">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="a1bdb-227">Int32</span><span class="sxs-lookup"><span data-stu-id="a1bdb-227">Int32</span></span>|<span data-ttu-id="a1bdb-228">O valor para o espaço livre mínimo em disco necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-228">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="a1bdb-229">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="a1bdb-229">minimumMemoryInMB</span></span>|<span data-ttu-id="a1bdb-230">Int32</span><span class="sxs-lookup"><span data-stu-id="a1bdb-230">Int32</span></span>|<span data-ttu-id="a1bdb-231">O valor da memória física mínima exigida para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-231">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="a1bdb-232">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="a1bdb-232">minimumNumberOfProcessors</span></span>|<span data-ttu-id="a1bdb-233">Int32</span><span class="sxs-lookup"><span data-stu-id="a1bdb-233">Int32</span></span>|<span data-ttu-id="a1bdb-234">O valor para o número mínimo de processadores necessários para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-234">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="a1bdb-235">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="a1bdb-235">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="a1bdb-236">Int32</span><span class="sxs-lookup"><span data-stu-id="a1bdb-236">Int32</span></span>|<span data-ttu-id="a1bdb-237">O valor para a velocidade de CPU mínima necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-237">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="a1bdb-238">detectionRules</span><span class="sxs-lookup"><span data-stu-id="a1bdb-238">detectionRules</span></span>|<span data-ttu-id="a1bdb-239">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-239">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="a1bdb-240">As regras de detecção para detectar o aplicativo de LoB (linha de negócios) do Win32.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-240">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a1bdb-241">installExperience</span><span class="sxs-lookup"><span data-stu-id="a1bdb-241">installExperience</span></span>|[<span data-ttu-id="a1bdb-242">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="a1bdb-242">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="a1bdb-243">A experiência de instalação para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-243">The install experience for this app.</span></span>|
|<span data-ttu-id="a1bdb-244">returnCodes</span><span class="sxs-lookup"><span data-stu-id="a1bdb-244">returnCodes</span></span>|<span data-ttu-id="a1bdb-245">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="a1bdb-245">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="a1bdb-246">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-246">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="a1bdb-247">msiInformation</span><span class="sxs-lookup"><span data-stu-id="a1bdb-247">msiInformation</span></span>|[<span data-ttu-id="a1bdb-248">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="a1bdb-248">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="a1bdb-249">Os detalhes do MSI, se este aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-249">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="a1bdb-250">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="a1bdb-250">setupFilePath</span></span>|<span data-ttu-id="a1bdb-251">String</span><span class="sxs-lookup"><span data-stu-id="a1bdb-251">String</span></span>|<span data-ttu-id="a1bdb-252">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-252">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="a1bdb-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1bdb-253">Response</span></span>
<span data-ttu-id="a1bdb-254">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-254">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1bdb-255">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1bdb-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1bdb-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1bdb-256">Request</span></span>
<span data-ttu-id="a1bdb-257">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2364

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
    "v10_1803": true
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

### <a name="response"></a><span data-ttu-id="a1bdb-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1bdb-258">Response</span></span>
<span data-ttu-id="a1bdb-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1bdb-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2536

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
    "v10_1803": true
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




