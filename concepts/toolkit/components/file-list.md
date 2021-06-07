---
title: Componente de lista de arquivos no microsoft Graph Toolkit
description: O componente de lista de arquivos é usado para exibir uma lista de arquivos mostrando seu ícone e nome
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: cfd4543cad98864a423699e4ed6cde7dc82ee6fb
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781090"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="46886-103">Componente de lista de arquivos no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="46886-103">File list component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="46886-104">O componente Lista [](/graph/api/resources/onedrive) de Arquivos exibe uma lista de várias pastas e arquivos usando o nome do arquivo/pasta, um ícone e outras propriedades que você especificar.</span><span class="sxs-lookup"><span data-stu-id="46886-104">The File List component displays [a list of multiple folders and files](/graph/api/resources/onedrive) by using the file/folder name, an icon, and other properties that you specify.</span></span> <span data-ttu-id="46886-105">Esse componente usa o [componente mgt-file.](./file.md)</span><span class="sxs-lookup"><span data-stu-id="46886-105">This component uses the [mgt-file](./file.md) component.</span></span> <span data-ttu-id="46886-106">Você pode especificar uma unidade ou site específico, exibir uma lista de arquivos com base no tipo de insight (tendência, usado ou compartilhado) ou fornecer consultas para uma lista personalizada de arquivos.</span><span class="sxs-lookup"><span data-stu-id="46886-106">You can specify a specific drive or site, display a list of files based on insight type (trending, used, or shared), or provide queries to a custom list of files.</span></span>

## <a name="example"></a><span data-ttu-id="46886-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46886-107">Example</span></span>

<span data-ttu-id="46886-108">O exemplo a seguir exibe um arquivo usando o `mgt-file-list` componente.</span><span class="sxs-lookup"><span data-stu-id="46886-108">The following example displays a file using the `mgt-file-list` component.</span></span> <span data-ttu-id="46886-109">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="46886-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[<span data-ttu-id="46886-110">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="46886-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a><span data-ttu-id="46886-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46886-111">Properties</span></span>

<span data-ttu-id="46886-112">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="46886-112">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="46886-113">Atributo</span><span class="sxs-lookup"><span data-stu-id="46886-113">Attribute</span></span> | <span data-ttu-id="46886-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46886-114">Property</span></span> | <span data-ttu-id="46886-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="46886-115">Description</span></span> |
| --------- | -------- | ----------- |
| <span data-ttu-id="46886-116">file-list-query</span><span class="sxs-lookup"><span data-stu-id="46886-116">file-list-query</span></span> | <span data-ttu-id="46886-117">fileListQuery</span><span class="sxs-lookup"><span data-stu-id="46886-117">fileListQuery</span></span> | <span data-ttu-id="46886-118">A consulta completa ou o caminho para a unidade ou site que contém a lista de arquivos a ser renderização.</span><span class="sxs-lookup"><span data-stu-id="46886-118">The full query or path to the drive or site that contains the list of files to render.</span></span> |
| <span data-ttu-id="46886-119">file-queries</span><span class="sxs-lookup"><span data-stu-id="46886-119">file-queries</span></span> | <span data-ttu-id="46886-120">fileQueries</span><span class="sxs-lookup"><span data-stu-id="46886-120">fileQueries</span></span> | <span data-ttu-id="46886-121">Uma matriz de consultas de arquivo a serem renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="46886-121">An array of file queries to be rendered by the component.</span></span> |
| <span data-ttu-id="46886-122">nenhuma</span><span class="sxs-lookup"><span data-stu-id="46886-122">none</span></span> | <span data-ttu-id="46886-123">arquivos</span><span class="sxs-lookup"><span data-stu-id="46886-123">files</span></span> | <span data-ttu-id="46886-124">Uma matriz de arquivos para obter ou definir a lista de arquivos renderizados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="46886-124">An array of files to get or set the list of files rendered by the component.</span></span> <span data-ttu-id="46886-125">Use isso para acessar os arquivos carregados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="46886-125">Use this to access the files loaded by the component.</span></span> <span data-ttu-id="46886-126">De definir esse valor para carregar seus próprios arquivos.</span><span class="sxs-lookup"><span data-stu-id="46886-126">Set this value to load your own files.</span></span> |
| <span data-ttu-id="46886-127">tipo de insight</span><span class="sxs-lookup"><span data-stu-id="46886-127">insight-type</span></span> | <span data-ttu-id="46886-128">insightType</span><span class="sxs-lookup"><span data-stu-id="46886-128">insightType</span></span> | <span data-ttu-id="46886-129">Definido para mostrar os arquivos de tendência, usados ou compartilhados do usuário.</span><span class="sxs-lookup"><span data-stu-id="46886-129">Set to show the user’s trending, used, or shared files.</span></span> |
| <span data-ttu-id="46886-130">drive-id</span><span class="sxs-lookup"><span data-stu-id="46886-130">drive-id</span></span> | <span data-ttu-id="46886-131">driveId</span><span class="sxs-lookup"><span data-stu-id="46886-131">driveId</span></span> | <span data-ttu-id="46886-132">ID da unidade à que a pasta pertence.</span><span class="sxs-lookup"><span data-stu-id="46886-132">ID of the drive the folder belongs to.</span></span> <span data-ttu-id="46886-133">Também deve fornecer um `item-id` ou `item-path` .</span><span class="sxs-lookup"><span data-stu-id="46886-133">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="46886-134">group-id</span><span class="sxs-lookup"><span data-stu-id="46886-134">group-id</span></span> | <span data-ttu-id="46886-135">groupId</span><span class="sxs-lookup"><span data-stu-id="46886-135">groupId</span></span> | <span data-ttu-id="46886-136">ID do grupo ao que a pasta pertence.</span><span class="sxs-lookup"><span data-stu-id="46886-136">ID of the group the folder belongs to.</span></span> <span data-ttu-id="46886-137">Também deve fornecer um `item-id` ou `item-path` .</span><span class="sxs-lookup"><span data-stu-id="46886-137">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="46886-138">site-id</span><span class="sxs-lookup"><span data-stu-id="46886-138">site-id</span></span> | <span data-ttu-id="46886-139">siteId</span><span class="sxs-lookup"><span data-stu-id="46886-139">siteId</span></span> | <span data-ttu-id="46886-140">ID do site ao que a pasta pertence.</span><span class="sxs-lookup"><span data-stu-id="46886-140">ID of the site the folder belongs to.</span></span> <span data-ttu-id="46886-141">Também deve fornecer um `{item-id}` ou `{item-path}` .</span><span class="sxs-lookup"><span data-stu-id="46886-141">Must also provide either `{item-id}` or `{item-path}`.</span></span> <span data-ttu-id="46886-142">Forneça `{list-id}` se você estiver fazendo referência a um arquivo de uma lista específica.</span><span class="sxs-lookup"><span data-stu-id="46886-142">Provide `{list-id}` if you’re referencing a file from a specific list.</span></span> |
| <span data-ttu-id="46886-143">item-id</span><span class="sxs-lookup"><span data-stu-id="46886-143">item-id</span></span> | <span data-ttu-id="46886-144">itemId</span><span class="sxs-lookup"><span data-stu-id="46886-144">itemId</span></span> | <span data-ttu-id="46886-145">ID da pasta.</span><span class="sxs-lookup"><span data-stu-id="46886-145">ID of the folder.</span></span> <span data-ttu-id="46886-146">A consulta padrão é `/me/drive/items` .</span><span class="sxs-lookup"><span data-stu-id="46886-146">Default query is `/me/drive/items`.</span></span> <span data-ttu-id="46886-147">Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico.</span><span class="sxs-lookup"><span data-stu-id="46886-147">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="46886-148">item-path</span><span class="sxs-lookup"><span data-stu-id="46886-148">item-path</span></span> | <span data-ttu-id="46886-149">itemPath</span><span class="sxs-lookup"><span data-stu-id="46886-149">itemPath</span></span> | <span data-ttu-id="46886-150">Caminho do item da pasta (em relação à raiz).</span><span class="sxs-lookup"><span data-stu-id="46886-150">Item path of the folder (relative to the root).</span></span> <span data-ttu-id="46886-151">A consulta padrão é `/me/drive/root` .</span><span class="sxs-lookup"><span data-stu-id="46886-151">Default query is `/me/drive/root`.</span></span> <span data-ttu-id="46886-152">Forneça `{drive-id}` , , ou para consultar um local `{group-id}` `{site-id}` `{user-id}` específico.</span><span class="sxs-lookup"><span data-stu-id="46886-152">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="46886-153">tamanho da página</span><span class="sxs-lookup"><span data-stu-id="46886-153">page-size</span></span> | <span data-ttu-id="46886-154">pageSize</span><span class="sxs-lookup"><span data-stu-id="46886-154">pageSize</span></span> | <span data-ttu-id="46886-155">Um valor de número para indicar o número máximo de arquivos a renderizar em cada página.</span><span class="sxs-lookup"><span data-stu-id="46886-155">A number value to indicate the maximum number of files to render on each page.</span></span> |
| <span data-ttu-id="46886-156">file-extensions</span><span class="sxs-lookup"><span data-stu-id="46886-156">file-extensions</span></span> | <span data-ttu-id="46886-157">fileExtensions</span><span class="sxs-lookup"><span data-stu-id="46886-157">fileExtensions</span></span> | <span data-ttu-id="46886-158">Uma matriz de extensões de arquivo usadas para filtrar arquivos para mostrar.</span><span class="sxs-lookup"><span data-stu-id="46886-158">An array of file extensions used to filter files to show.</span></span> |
| <span data-ttu-id="46886-159">hide-more-files-button</span><span class="sxs-lookup"><span data-stu-id="46886-159">hide-more-files-button</span></span> | <span data-ttu-id="46886-160">hideMoreFilesButton</span><span class="sxs-lookup"><span data-stu-id="46886-160">hideMoreFilesButton</span></span> | <span data-ttu-id="46886-161">Um booleano para indicar se é preciso mostrar um botão para renderizar mais arquivos.</span><span class="sxs-lookup"><span data-stu-id="46886-161">A boolean to indicate whether to show a button to render more files.</span></span> |

<span data-ttu-id="46886-162">O exemplo a seguir altera o comportamento do componente para buscar uma lista de arquivos de uma consulta específica.</span><span class="sxs-lookup"><span data-stu-id="46886-162">The following example changes the behavior of the component to fetch a file list from a specific query.</span></span>

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

<span data-ttu-id="46886-163">O exemplo a seguir altera o comportamento do componente para buscar uma lista de arquivos de uma pasta fornecendo a id da pasta.</span><span class="sxs-lookup"><span data-stu-id="46886-163">The following example changes the behavior of the component to fetch a file list from a folder by providing the folder id.</span></span>

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

<span data-ttu-id="46886-164">O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos de um grupo fornecendo a id do grupo e o caminho da pasta.</span><span class="sxs-lookup"><span data-stu-id="46886-164">The following example changes the behavior of the component to fetch file list from a group by providing the group id and folder path.</span></span>

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

<span data-ttu-id="46886-165">O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos de um usuário, fornecendo a ID do usuário e a id da pasta.</span><span class="sxs-lookup"><span data-stu-id="46886-165">The following example changes the behavior of the component to fetch file list from a user by providing the user id and folder id.</span></span>

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

<span data-ttu-id="46886-166">O exemplo a seguir altera o comportamento do componente para buscar a lista de arquivos fornecendo o tipo de insight.</span><span class="sxs-lookup"><span data-stu-id="46886-166">The following example changes the behavior of the component to fetch file list by providing the insight type.</span></span>

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="methods"></a><span data-ttu-id="46886-167">Métodos</span><span class="sxs-lookup"><span data-stu-id="46886-167">Methods</span></span>
| <span data-ttu-id="46886-168">Método</span><span class="sxs-lookup"><span data-stu-id="46886-168">Method</span></span> | <span data-ttu-id="46886-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="46886-169">Description</span></span> |
| --- | --- |
| <span data-ttu-id="46886-170">reload(clearCache = false)</span><span class="sxs-lookup"><span data-stu-id="46886-170">reload(clearCache = false)</span></span> | <span data-ttu-id="46886-171">Chame o método para recarregar o componente com novos dados potenciais com base em suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="46886-171">Call the method to reload the component with potential new data based on its properties.</span></span> <span data-ttu-id="46886-172">Passe `true` para limpar o cache antes de recarregar.</span><span class="sxs-lookup"><span data-stu-id="46886-172">Pass `true` to clear the cache before reloading.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="46886-173">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="46886-173">CSS custom properties</span></span>

<span data-ttu-id="46886-174">O `mgt-file-list` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="46886-174">The `mgt-file-list` component defines the following CSS custom properties.</span></span>

```css
mgt-file-list {
  --font-family: 'Segoe UI';
  --font-size: 14px;

  --file-list-background-color: #ffffff;
  --file-list-border: none;
  --file-list-box-shadow: none;
  --file-list-padding: 4px 0;
  --file-list-margin: 0;

  --file-item-background-color--hover: rgba(0, 0, 0, 0.1);
  --file-item-background-color--active: rgba(0, 0, 0, 0.05);
  --file-item-border-radius: 2px;
  --file-item-margin: 0 4px;

  --file-item-border-top: none;
  --file-item-border-left: none;
  --file-item-border-right: none;
  --file-item-border-bottom: none;

  --show-more-button-background-color: #f3f2f1;
  --show-more-button-background-color--hover: rgba(0, 0, 0, 0.1);
  --show-more-button-font-size: 12px;
  --show-more-button-padding: 6px;
  --show-more-button-border-bottom-right-radius: 4px;
  --show-more-button-border-bottom-left-radius: 4px;
}
```

<span data-ttu-id="46886-175">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="46886-175">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="46886-176">ApIs Graph Microsoft e permissões</span><span class="sxs-lookup"><span data-stu-id="46886-176">Microsoft Graph APIs and permissions</span></span>

| <span data-ttu-id="46886-177">Configuração</span><span class="sxs-lookup"><span data-stu-id="46886-177">Configuration</span></span> | <span data-ttu-id="46886-178">Permissões</span><span class="sxs-lookup"><span data-stu-id="46886-178">Permissions</span></span> | <span data-ttu-id="46886-179">API</span><span class="sxs-lookup"><span data-stu-id="46886-179">API</span></span> |
| ------------- | ----------------- | --- |
| <span data-ttu-id="46886-180">Padrão (nenhum identificador ou consulta fornecida)</span><span class="sxs-lookup"><span data-stu-id="46886-180">Default (no identifiers or query provided)</span></span> | <span data-ttu-id="46886-181">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-181">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root/children` |
| <span data-ttu-id="46886-182">Fornecer `{drive-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="46886-182">Provide `{drive-id}` AND `{item-id}`</span></span> | <span data-ttu-id="46886-183">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-183">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/items/{item-id}/children` |
| <span data-ttu-id="46886-184">Fornecer `{group-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="46886-184">Provide `{group-id}` AND `{item-id}`</span></span> | <span data-ttu-id="46886-185">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-185">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="46886-186">Fornecer SOMENTE `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="46886-186">Provide ONLY `{item-id}`</span></span> | <span data-ttu-id="46886-187">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-187">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/items/{item-id}/children` |
| <span data-ttu-id="46886-188">Fornecer `{site-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="46886-188">Provide `{site-id}` AND `{item-id}`</span></span> | <span data-ttu-id="46886-189">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-189">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="46886-190">Pprovide `{user-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="46886-190">Pprovide `{user-id}` AND `{item-id}`</span></span> | <span data-ttu-id="46886-191">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-191">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="46886-192">Fornecer `{drive-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="46886-192">Provide `{drive-id}` AND `{item-path}`</span></span> | <span data-ttu-id="46886-193">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-193">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| <span data-ttu-id="46886-194">Fornecer `{group-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="46886-194">Provide `{group-id}` AND `{item-path}`</span></span> | <span data-ttu-id="46886-195">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-195">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/root:/{item-path}:/children` |
| <span data-ttu-id="46886-196">Fornecer `{site-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="46886-196">Provide `{site-id}` AND `{item-path}`</span></span> | <span data-ttu-id="46886-197">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-197">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/root:/{item-path}:/children` |
| <span data-ttu-id="46886-198">Fornecer `{user-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="46886-198">Provide `{user-id}` AND `{item-path}`</span></span> | <span data-ttu-id="46886-199">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-199">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/root:/{item-path}:/children` |
| <span data-ttu-id="46886-200">Fornecer somente `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="46886-200">Provide only `{item-path}`</span></span> | <span data-ttu-id="46886-201">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-201">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root:/{item-path}:/children` |
| <span data-ttu-id="46886-202">`insight-type` é definido como tendência</span><span class="sxs-lookup"><span data-stu-id="46886-202">`insight-type` is set to trending</span></span> | <span data-ttu-id="46886-203">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-203">Sites.Read.All</span></span> | `GET /me/insights/trending` |
| <span data-ttu-id="46886-204">Fornecer `{user-id or upn}` AND está definido `insight-type` como `trending`</span><span class="sxs-lookup"><span data-stu-id="46886-204">Provide `{user-id or upn}` AND `insight-type` is set to `trending`</span></span> | <span data-ttu-id="46886-205">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-205">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/trending` |
| <span data-ttu-id="46886-206">`insight-type` está definido como `used`</span><span class="sxs-lookup"><span data-stu-id="46886-206">`insight-type` is set to `used`</span></span> | <span data-ttu-id="46886-207">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-207">Sites.Read.All</span></span> | `GET /me/insights/used` |
| <span data-ttu-id="46886-208">Fornecer `{user-id or upn}` AND está definido `insight-type` como `used`</span><span class="sxs-lookup"><span data-stu-id="46886-208">Provide `{user-id or upn}` AND `insight-type` is set to `used`</span></span> | <span data-ttu-id="46886-209">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-209">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/used` |
| <span data-ttu-id="46886-210">`insight-type` é definido como compartilhado</span><span class="sxs-lookup"><span data-stu-id="46886-210">`insight-type` is set to shared</span></span> | <span data-ttu-id="46886-211">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-211">Sites.Read.All</span></span> | `GET /me/insights/shared` |
| <span data-ttu-id="46886-212">Fornecer `{user-id or upn}` AND está definido `insight-type` como `shared`</span><span class="sxs-lookup"><span data-stu-id="46886-212">Provide `{user-id or upn}` AND `insight-type` is set to `shared`</span></span> | <span data-ttu-id="46886-213">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="46886-213">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a><span data-ttu-id="46886-214">Eventos</span><span class="sxs-lookup"><span data-stu-id="46886-214">Events</span></span>

| <span data-ttu-id="46886-215">Evento</span><span class="sxs-lookup"><span data-stu-id="46886-215">Event</span></span> | <span data-ttu-id="46886-216">Descrição</span><span class="sxs-lookup"><span data-stu-id="46886-216">Description</span></span> |
| ----- | ----------- |
| <span data-ttu-id="46886-217">itemClick</span><span class="sxs-lookup"><span data-stu-id="46886-217">itemClick</span></span> | <span data-ttu-id="46886-218">Disparado quando o usuário clica em um arquivo.</span><span class="sxs-lookup"><span data-stu-id="46886-218">Fired when the user clicks a file.</span></span> <span data-ttu-id="46886-219">Retorna os detalhes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="46886-219">Returns the file details.</span></span> |

## <a name="templates"></a><span data-ttu-id="46886-220">Modelos</span><span class="sxs-lookup"><span data-stu-id="46886-220">Templates</span></span>

<span data-ttu-id="46886-221">O `mgt-file-list` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="46886-221">The `mgt-file-list` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="46886-222">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o valor como um dos tipos de dados `<template>` `data-type` listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="46886-222">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the data types listed in the following table.</span></span>

| <span data-ttu-id="46886-223">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="46886-223">Data type</span></span> | <span data-ttu-id="46886-224">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="46886-224">Data context</span></span> | <span data-ttu-id="46886-225">Descrição</span><span class="sxs-lookup"><span data-stu-id="46886-225">Description</span></span> |
| ----------- | -------------- | ------------ |
| <span data-ttu-id="46886-226">Padrão.</span><span class="sxs-lookup"><span data-stu-id="46886-226">default</span></span> | <span data-ttu-id="46886-227">`files`: lista de objetos de arquivo</span><span class="sxs-lookup"><span data-stu-id="46886-227">`files`: list of file objects</span></span> | <span data-ttu-id="46886-228">O modelo padrão substitui todo o componente por seu próprio.</span><span class="sxs-lookup"><span data-stu-id="46886-228">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="46886-229">file</span><span class="sxs-lookup"><span data-stu-id="46886-229">file</span></span> | <span data-ttu-id="46886-230">`file`: objeto file</span><span class="sxs-lookup"><span data-stu-id="46886-230">`file`: file object</span></span> | <span data-ttu-id="46886-231">O modelo usado para renderizar cada arquivo.</span><span class="sxs-lookup"><span data-stu-id="46886-231">The template used to render each file.</span></span> |
| <span data-ttu-id="46886-232">no-data</span><span class="sxs-lookup"><span data-stu-id="46886-232">no-data</span></span> | <span data-ttu-id="46886-233">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="46886-233">No data context is passed</span></span> | <span data-ttu-id="46886-234">O modelo usado quando nenhum dado está disponível.</span><span class="sxs-lookup"><span data-stu-id="46886-234">The template used when no data is available.</span></span> |
| <span data-ttu-id="46886-235">loading</span><span class="sxs-lookup"><span data-stu-id="46886-235">loading</span></span> | <span data-ttu-id="46886-236">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="46886-236">No data context is passed</span></span> | <span data-ttu-id="46886-237">O modelo usado enquanto o componente carrega o estado.</span><span class="sxs-lookup"><span data-stu-id="46886-237">The template used while the component loads state.</span></span> |

## <a name="authentication"></a><span data-ttu-id="46886-238">Autenticação</span><span class="sxs-lookup"><span data-stu-id="46886-238">Authentication</span></span>

<span data-ttu-id="46886-239">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="46886-239">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="46886-240">Cache</span><span class="sxs-lookup"><span data-stu-id="46886-240">Cache</span></span>

|<span data-ttu-id="46886-241">Armazenamento de objetos</span><span class="sxs-lookup"><span data-stu-id="46886-241">Object store</span></span>|<span data-ttu-id="46886-242">Dados armazenados em cache</span><span class="sxs-lookup"><span data-stu-id="46886-242">Cached data</span></span>|<span data-ttu-id="46886-243">Comentários</span><span class="sxs-lookup"><span data-stu-id="46886-243">Remarks</span></span>|
|---------|-----------|-------|
|`fileLists`|<span data-ttu-id="46886-244">Lista de listas de arquivos</span><span class="sxs-lookup"><span data-stu-id="46886-244">List of file lists</span></span>|<span data-ttu-id="46886-245">Lista de cache padrão para armazenar listas de arquivos.</span><span class="sxs-lookup"><span data-stu-id="46886-245">Default cache list to store file lists.</span></span>|
|`insightfileLists`|<span data-ttu-id="46886-246">Lista de listas de arquivos de insight</span><span class="sxs-lookup"><span data-stu-id="46886-246">List of insight file lists</span></span>|<span data-ttu-id="46886-247">Usado quando `insightType` fornecido.</span><span class="sxs-lookup"><span data-stu-id="46886-247">Used when `insightType` is provided.</span></span>|

> [!NOTE]
> <span data-ttu-id="46886-248">O `mgt-file-list` componente também usa o armazenamento de objetos em `fileQueries` `mgt-file` IndexedDB para armazenar arquivos em cache quando `fileQueries` é fornecido.</span><span class="sxs-lookup"><span data-stu-id="46886-248">The `mgt-file-list` component also uses the `fileQueries` object store in `mgt-file` IndexedDB to cache files when `fileQueries` is provided.</span></span>

<span data-ttu-id="46886-249">Para obter detalhes sobre como configurar o cache, [consulte Caching](../customize-components/cache.md).</span><span class="sxs-lookup"><span data-stu-id="46886-249">For details about how to configure the cache, see [Caching](../customize-components/cache.md).</span></span>