---
ms.localizationpriority: medium
ms.openlocfilehash: 48b73a117c130f786a72bbc554632b0a858ebab7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289487"
---
<!-- markdownlint-disable MD041-->

Quando um aplicativo consulta uma relação que retorna uma coleção de tipo directoryObject, caso não tenha permissão para ler determinado tipo (como dispositivo), os membros desse tipo são retornados, mas com informações limitadas. Com esse comportamento, os aplicativos podem solicitar as permissões menos privilegiadas de que precisam, em vez de depender do conjunto de *Diretório.** permissões. Para obter mais detalhes, confira [Informações limitadas retornadas para objetos membro inacessíveis](/graph/permissions-reference#limited-information-returned-for-inaccessible-member-objects).
