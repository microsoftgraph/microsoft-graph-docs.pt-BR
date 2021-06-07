---
title: Criar win32LobApp
description: Crie um novo objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4720cd7b77ce32e059a5e2754534efee619cfd79
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756740"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="a724a-103">Criar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="a724a-103">Create win32LobApp</span></span>

<span data-ttu-id="a724a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a724a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a724a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a724a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a724a-106">Crie um novo [objeto win32LobApp.](../resources/intune-apps-win32lobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a724a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a724a-107">Prerequisites</span></span>
<span data-ttu-id="a724a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a724a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a724a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a724a-110">Permission type</span></span>|<span data-ttu-id="a724a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a724a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a724a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a724a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a724a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a724a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a724a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a724a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a724a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a724a-115">Not supported.</span></span>|
|<span data-ttu-id="a724a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a724a-116">Application</span></span>|<span data-ttu-id="a724a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a724a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a724a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a724a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a724a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a724a-119">Request headers</span></span>
|<span data-ttu-id="a724a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a724a-120">Header</span></span>|<span data-ttu-id="a724a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a724a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a724a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a724a-122">Authorization</span></span>|<span data-ttu-id="a724a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a724a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a724a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a724a-124">Accept</span></span>|<span data-ttu-id="a724a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a724a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a724a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a724a-126">Request body</span></span>
<span data-ttu-id="a724a-127">No corpo da solicitação, fornece uma representação JSON para o objeto win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="a724a-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="a724a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar o win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="a724a-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="a724a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a724a-129">Property</span></span>|<span data-ttu-id="a724a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a724a-130">Type</span></span>|<span data-ttu-id="a724a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a724a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a724a-132">id</span><span class="sxs-lookup"><span data-stu-id="a724a-132">id</span></span>|<span data-ttu-id="a724a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a724a-133">String</span></span>|<span data-ttu-id="a724a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a724a-134">Key of the entity.</span></span> <span data-ttu-id="a724a-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a724a-136">displayName</span></span>|<span data-ttu-id="a724a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a724a-137">String</span></span>|<span data-ttu-id="a724a-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a724a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a724a-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-140">descrição</span><span class="sxs-lookup"><span data-stu-id="a724a-140">description</span></span>|<span data-ttu-id="a724a-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a724a-141">String</span></span>|<span data-ttu-id="a724a-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-142">The description of the app.</span></span> <span data-ttu-id="a724a-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-144">publicador</span><span class="sxs-lookup"><span data-stu-id="a724a-144">publisher</span></span>|<span data-ttu-id="a724a-145">String</span><span class="sxs-lookup"><span data-stu-id="a724a-145">String</span></span>|<span data-ttu-id="a724a-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-146">The publisher of the app.</span></span> <span data-ttu-id="a724a-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a724a-148">largeIcon</span></span>|[<span data-ttu-id="a724a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a724a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a724a-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="a724a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a724a-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a724a-152">createdDateTime</span></span>|<span data-ttu-id="a724a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a724a-153">DateTimeOffset</span></span>|<span data-ttu-id="a724a-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-154">The date and time the app was created.</span></span> <span data-ttu-id="a724a-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a724a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a724a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a724a-157">DateTimeOffset</span></span>|<span data-ttu-id="a724a-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a724a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a724a-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a724a-160">isFeatured</span></span>|<span data-ttu-id="a724a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a724a-161">Boolean</span></span>|<span data-ttu-id="a724a-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a724a-163">privacyInformationUrl</span></span>|<span data-ttu-id="a724a-164">String</span><span class="sxs-lookup"><span data-stu-id="a724a-164">String</span></span>|<span data-ttu-id="a724a-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="a724a-165">The privacy statement Url.</span></span> <span data-ttu-id="a724a-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a724a-167">informationUrl</span></span>|<span data-ttu-id="a724a-168">String</span><span class="sxs-lookup"><span data-stu-id="a724a-168">String</span></span>|<span data-ttu-id="a724a-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a724a-169">The more information Url.</span></span> <span data-ttu-id="a724a-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="a724a-171">owner</span></span>|<span data-ttu-id="a724a-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a724a-172">String</span></span>|<span data-ttu-id="a724a-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a724a-173">The owner of the app.</span></span> <span data-ttu-id="a724a-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-175">developer</span><span class="sxs-lookup"><span data-stu-id="a724a-175">developer</span></span>|<span data-ttu-id="a724a-176">String</span><span class="sxs-lookup"><span data-stu-id="a724a-176">String</span></span>|<span data-ttu-id="a724a-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-177">The developer of the app.</span></span> <span data-ttu-id="a724a-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-179">notes</span><span class="sxs-lookup"><span data-stu-id="a724a-179">notes</span></span>|<span data-ttu-id="a724a-180">String</span><span class="sxs-lookup"><span data-stu-id="a724a-180">String</span></span>|<span data-ttu-id="a724a-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-181">Notes for the app.</span></span> <span data-ttu-id="a724a-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a724a-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="a724a-183">publishingState</span></span>|[<span data-ttu-id="a724a-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a724a-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a724a-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-185">The publishing state for the app.</span></span> <span data-ttu-id="a724a-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="a724a-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a724a-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a724a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a724a-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a724a-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a724a-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a724a-189">committedContentVersion</span></span>|<span data-ttu-id="a724a-190">String</span><span class="sxs-lookup"><span data-stu-id="a724a-190">String</span></span>|<span data-ttu-id="a724a-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="a724a-191">The internal committed content version.</span></span> <span data-ttu-id="a724a-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a724a-193">fileName</span><span class="sxs-lookup"><span data-stu-id="a724a-193">fileName</span></span>|<span data-ttu-id="a724a-194">String</span><span class="sxs-lookup"><span data-stu-id="a724a-194">String</span></span>|<span data-ttu-id="a724a-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="a724a-195">The name of the main Lob application file.</span></span> <span data-ttu-id="a724a-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a724a-197">size</span><span class="sxs-lookup"><span data-stu-id="a724a-197">size</span></span>|<span data-ttu-id="a724a-198">Int64</span><span class="sxs-lookup"><span data-stu-id="a724a-198">Int64</span></span>|<span data-ttu-id="a724a-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="a724a-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="a724a-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a724a-201">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="a724a-201">installCommandLine</span></span>|<span data-ttu-id="a724a-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a724a-202">String</span></span>|<span data-ttu-id="a724a-203">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="a724a-203">The command line to install this app</span></span>|
|<span data-ttu-id="a724a-204">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="a724a-204">uninstallCommandLine</span></span>|<span data-ttu-id="a724a-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a724a-205">String</span></span>|<span data-ttu-id="a724a-206">A linha de comando para desinstalar esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="a724a-206">The command line to uninstall this app</span></span>|
|<span data-ttu-id="a724a-207">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="a724a-207">applicableArchitectures</span></span>|[<span data-ttu-id="a724a-208">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a724a-208">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a724a-209">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="a724a-209">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="a724a-210">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="a724a-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="a724a-211">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="a724a-211">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="a724a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a724a-212">Int32</span></span>|<span data-ttu-id="a724a-213">O valor do espaço em disco gratuito mínimo necessário para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-213">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="a724a-214">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="a724a-214">minimumMemoryInMB</span></span>|<span data-ttu-id="a724a-215">Int32</span><span class="sxs-lookup"><span data-stu-id="a724a-215">Int32</span></span>|<span data-ttu-id="a724a-216">O valor da memória física mínima necessária para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-216">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="a724a-217">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="a724a-217">minimumNumberOfProcessors</span></span>|<span data-ttu-id="a724a-218">Int32</span><span class="sxs-lookup"><span data-stu-id="a724a-218">Int32</span></span>|<span data-ttu-id="a724a-219">O valor do número mínimo de processadores necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-219">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="a724a-220">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="a724a-220">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="a724a-221">Int32</span><span class="sxs-lookup"><span data-stu-id="a724a-221">Int32</span></span>|<span data-ttu-id="a724a-222">O valor da velocidade mínima da CPU necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-222">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="a724a-223">rules</span><span class="sxs-lookup"><span data-stu-id="a724a-223">rules</span></span>|<span data-ttu-id="a724a-224">[Coleção win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="a724a-225">As regras de detecção e requisitos para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-225">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="a724a-226">installExperience</span><span class="sxs-lookup"><span data-stu-id="a724a-226">installExperience</span></span>|[<span data-ttu-id="a724a-227">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="a724a-227">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="a724a-228">A experiência de instalação deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a724a-228">The install experience for this app.</span></span>|
|<span data-ttu-id="a724a-229">returnCodes</span><span class="sxs-lookup"><span data-stu-id="a724a-229">returnCodes</span></span>|<span data-ttu-id="a724a-230">[Coleção win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="a724a-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="a724a-231">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="a724a-231">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="a724a-232">msiInformation</span><span class="sxs-lookup"><span data-stu-id="a724a-232">msiInformation</span></span>|[<span data-ttu-id="a724a-233">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="a724a-233">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="a724a-234">O MSI detalha se esse aplicativo Win32 é um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="a724a-234">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="a724a-235">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="a724a-235">setupFilePath</span></span>|<span data-ttu-id="a724a-236">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a724a-236">String</span></span>|<span data-ttu-id="a724a-237">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="a724a-237">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="a724a-238">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="a724a-238">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="a724a-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a724a-239">String</span></span>|<span data-ttu-id="a724a-240">O valor da versão mínima com suporte do Windows.</span><span class="sxs-lookup"><span data-stu-id="a724a-240">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="a724a-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="a724a-241">Response</span></span>
<span data-ttu-id="a724a-242">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a724a-242">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a724a-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a724a-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="a724a-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a724a-244">Request</span></span>
<span data-ttu-id="a724a-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a724a-245">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a724a-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="a724a-246">Response</span></span>
<span data-ttu-id="a724a-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a724a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




