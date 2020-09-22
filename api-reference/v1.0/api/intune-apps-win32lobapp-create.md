---
title: Criar win32LobApp
description: Criar um novo objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c903de1e1f2bec92c255d29878eac06d38f4428c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080027"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="8c5d0-103">Criar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="8c5d0-103">Create win32LobApp</span></span>

<span data-ttu-id="8c5d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c5d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c5d0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c5d0-106">Criar um novo objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8c5d0-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c5d0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c5d0-107">Prerequisites</span></span>
<span data-ttu-id="8c5d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c5d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c5d0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c5d0-110">Permission type</span></span>|<span data-ttu-id="8c5d0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c5d0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c5d0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c5d0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c5d0-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c5d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-115">Not supported.</span></span>|
|<span data-ttu-id="8c5d0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c5d0-116">Application</span></span>|<span data-ttu-id="8c5d0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c5d0-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c5d0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c5d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8c5d0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c5d0-119">Request headers</span></span>
|<span data-ttu-id="8c5d0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c5d0-120">Header</span></span>|<span data-ttu-id="8c5d0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8c5d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c5d0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c5d0-122">Authorization</span></span>|<span data-ttu-id="8c5d0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c5d0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c5d0-124">Accept</span></span>|<span data-ttu-id="8c5d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c5d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c5d0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c5d0-126">Request body</span></span>
<span data-ttu-id="8c5d0-127">No corpo da solicitação, forneça uma representação JSON do objeto win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="8c5d0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="8c5d0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c5d0-129">Property</span></span>|<span data-ttu-id="8c5d0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c5d0-130">Type</span></span>|<span data-ttu-id="8c5d0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c5d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c5d0-132">id</span><span class="sxs-lookup"><span data-stu-id="8c5d0-132">id</span></span>|<span data-ttu-id="8c5d0-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c5d0-133">String</span></span>|<span data-ttu-id="8c5d0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-134">Key of the entity.</span></span> <span data-ttu-id="8c5d0-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8c5d0-136">displayName</span></span>|<span data-ttu-id="8c5d0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c5d0-137">String</span></span>|<span data-ttu-id="8c5d0-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8c5d0-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-140">description</span><span class="sxs-lookup"><span data-stu-id="8c5d0-140">description</span></span>|<span data-ttu-id="8c5d0-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c5d0-141">String</span></span>|<span data-ttu-id="8c5d0-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-142">The description of the app.</span></span> <span data-ttu-id="8c5d0-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-144">publicador</span><span class="sxs-lookup"><span data-stu-id="8c5d0-144">publisher</span></span>|<span data-ttu-id="8c5d0-145">String</span><span class="sxs-lookup"><span data-stu-id="8c5d0-145">String</span></span>|<span data-ttu-id="8c5d0-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-146">The publisher of the app.</span></span> <span data-ttu-id="8c5d0-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8c5d0-148">largeIcon</span></span>|[<span data-ttu-id="8c5d0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8c5d0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8c5d0-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8c5d0-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c5d0-152">createdDateTime</span></span>|<span data-ttu-id="8c5d0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c5d0-153">DateTimeOffset</span></span>|<span data-ttu-id="8c5d0-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-154">The date and time the app was created.</span></span> <span data-ttu-id="8c5d0-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c5d0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8c5d0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c5d0-157">DateTimeOffset</span></span>|<span data-ttu-id="8c5d0-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8c5d0-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8c5d0-160">isFeatured</span></span>|<span data-ttu-id="8c5d0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c5d0-161">Boolean</span></span>|<span data-ttu-id="8c5d0-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8c5d0-163">privacyInformationUrl</span></span>|<span data-ttu-id="8c5d0-164">String</span><span class="sxs-lookup"><span data-stu-id="8c5d0-164">String</span></span>|<span data-ttu-id="8c5d0-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-165">The privacy statement Url.</span></span> <span data-ttu-id="8c5d0-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8c5d0-167">informationUrl</span></span>|<span data-ttu-id="8c5d0-168">String</span><span class="sxs-lookup"><span data-stu-id="8c5d0-168">String</span></span>|<span data-ttu-id="8c5d0-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-169">The more information Url.</span></span> <span data-ttu-id="8c5d0-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-171">owner</span><span class="sxs-lookup"><span data-stu-id="8c5d0-171">owner</span></span>|<span data-ttu-id="8c5d0-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c5d0-172">String</span></span>|<span data-ttu-id="8c5d0-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-173">The owner of the app.</span></span> <span data-ttu-id="8c5d0-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-175">developer</span><span class="sxs-lookup"><span data-stu-id="8c5d0-175">developer</span></span>|<span data-ttu-id="8c5d0-176">String</span><span class="sxs-lookup"><span data-stu-id="8c5d0-176">String</span></span>|<span data-ttu-id="8c5d0-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-177">The developer of the app.</span></span> <span data-ttu-id="8c5d0-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-179">notes</span><span class="sxs-lookup"><span data-stu-id="8c5d0-179">notes</span></span>|<span data-ttu-id="8c5d0-180">String</span><span class="sxs-lookup"><span data-stu-id="8c5d0-180">String</span></span>|<span data-ttu-id="8c5d0-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-181">Notes for the app.</span></span> <span data-ttu-id="8c5d0-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c5d0-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="8c5d0-183">publishingState</span></span>|[<span data-ttu-id="8c5d0-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8c5d0-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8c5d0-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-185">The publishing state for the app.</span></span> <span data-ttu-id="8c5d0-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8c5d0-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c5d0-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8c5d0-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8c5d0-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8c5d0-189">committedContentVersion</span></span>|<span data-ttu-id="8c5d0-190">String</span><span class="sxs-lookup"><span data-stu-id="8c5d0-190">String</span></span>|<span data-ttu-id="8c5d0-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-191">The internal committed content version.</span></span> <span data-ttu-id="8c5d0-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8c5d0-193">fileName</span><span class="sxs-lookup"><span data-stu-id="8c5d0-193">fileName</span></span>|<span data-ttu-id="8c5d0-194">String</span><span class="sxs-lookup"><span data-stu-id="8c5d0-194">String</span></span>|<span data-ttu-id="8c5d0-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-195">The name of the main Lob application file.</span></span> <span data-ttu-id="8c5d0-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8c5d0-197">size</span><span class="sxs-lookup"><span data-stu-id="8c5d0-197">size</span></span>|<span data-ttu-id="8c5d0-198">Int64</span><span class="sxs-lookup"><span data-stu-id="8c5d0-198">Int64</span></span>|<span data-ttu-id="8c5d0-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="8c5d0-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8c5d0-201">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="8c5d0-201">installCommandLine</span></span>|<span data-ttu-id="8c5d0-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c5d0-202">String</span></span>|<span data-ttu-id="8c5d0-203">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c5d0-203">The command line to install this app</span></span>|
|<span data-ttu-id="8c5d0-204">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="8c5d0-204">uninstallCommandLine</span></span>|<span data-ttu-id="8c5d0-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c5d0-205">String</span></span>|<span data-ttu-id="8c5d0-206">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c5d0-206">The command line to uninstall this app</span></span>|
|<span data-ttu-id="8c5d0-207">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="8c5d0-207">applicableArchitectures</span></span>|[<span data-ttu-id="8c5d0-208">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="8c5d0-208">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="8c5d0-209">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-209">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="8c5d0-210">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="8c5d0-211">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="8c5d0-211">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="8c5d0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5d0-212">Int32</span></span>|<span data-ttu-id="8c5d0-213">O valor para o espaço livre mínimo em disco necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-213">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="8c5d0-214">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="8c5d0-214">minimumMemoryInMB</span></span>|<span data-ttu-id="8c5d0-215">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5d0-215">Int32</span></span>|<span data-ttu-id="8c5d0-216">O valor da memória física mínima exigida para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-216">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="8c5d0-217">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="8c5d0-217">minimumNumberOfProcessors</span></span>|<span data-ttu-id="8c5d0-218">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5d0-218">Int32</span></span>|<span data-ttu-id="8c5d0-219">O valor para o número mínimo de processadores necessários para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-219">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="8c5d0-220">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="8c5d0-220">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="8c5d0-221">Int32</span><span class="sxs-lookup"><span data-stu-id="8c5d0-221">Int32</span></span>|<span data-ttu-id="8c5d0-222">O valor para a velocidade de CPU mínima necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-222">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="8c5d0-223">regras</span><span class="sxs-lookup"><span data-stu-id="8c5d0-223">rules</span></span>|<span data-ttu-id="8c5d0-224">coleção [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="8c5d0-225">As regras de detecção e requisitos para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-225">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="8c5d0-226">installExperience</span><span class="sxs-lookup"><span data-stu-id="8c5d0-226">installExperience</span></span>|[<span data-ttu-id="8c5d0-227">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="8c5d0-227">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="8c5d0-228">A experiência de instalação para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-228">The install experience for this app.</span></span>|
|<span data-ttu-id="8c5d0-229">returnCodes</span><span class="sxs-lookup"><span data-stu-id="8c5d0-229">returnCodes</span></span>|<span data-ttu-id="8c5d0-230">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="8c5d0-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="8c5d0-231">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-231">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="8c5d0-232">msiInformation</span><span class="sxs-lookup"><span data-stu-id="8c5d0-232">msiInformation</span></span>|[<span data-ttu-id="8c5d0-233">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="8c5d0-233">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="8c5d0-234">Os detalhes do MSI, se este aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-234">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="8c5d0-235">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="8c5d0-235">setupFilePath</span></span>|<span data-ttu-id="8c5d0-236">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c5d0-236">String</span></span>|<span data-ttu-id="8c5d0-237">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-237">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="8c5d0-238">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="8c5d0-238">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="8c5d0-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c5d0-239">String</span></span>|<span data-ttu-id="8c5d0-240">O valor da versão mínima com suporte do Windows.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-240">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="8c5d0-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c5d0-241">Response</span></span>
<span data-ttu-id="8c5d0-242">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-242">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c5d0-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c5d0-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c5d0-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c5d0-244">Request</span></span>
<span data-ttu-id="8c5d0-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2134

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
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
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```

### <a name="response"></a><span data-ttu-id="8c5d0-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c5d0-246">Response</span></span>
<span data-ttu-id="8c5d0-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c5d0-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2306

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
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
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```






