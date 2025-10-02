import heapq

# Использование встроенного модуля
numbers = [8, 3, 5, 1, 6, 2, 4, 7]
heapq.heapify(numbers)
heapq.heappush(numbers, 0)
min_val = heapq.heappop(numbers)

# Кастомная реализация
class BinaryHeap:
    def __init__(self):
        self.heap = []
    
    def insert(self, key):
        self.heap.append(key)
        self._heapify_up(len(self.heap) - 1)
    
    def delete_min(self):
        if not self.heap:
            return None
        min_val = self.heap[0]
        self.heap[0] = self.heap[-1]
        self.heap.pop()
        self._heapify_down(0)
        return min_val
